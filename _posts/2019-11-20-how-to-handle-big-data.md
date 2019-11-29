---
title: "How to handle big data"
author: Daoud Clarke
excerpt: "Think again before reaching for the big data tools."
header:
  overlay_image: /assets/images/header-article.jpg
  overlay_filter: 0.6
---

There's a lot of hype about big data. The problem of handling big data
is technically interesting, so a lot of effort has been put into
building tools to handle big data.

As data scientists, we have to think carefully about when it is
appropriate to use these tools, and when we can be more effective
without them. In this article I'll talk about some tactics for
approaching a problem when big data is involved.

# 1. What type of problem is it?

The first step in handling big data is to take a step back and
think. Being big makes everything slow, so it's worth spending time
thinking before you start the slow thing, because thinking can make it
orders of magnitude faster.

The first thing to think about is what type of problem you have. If
it's a data science problem you're tackling, it's probably either some
kind of analysis or a machine learning experiment you need to
perform. (Other problems are outside the scope of this article!)

How big is the problem? Will you need to access the data often, or
will a one-off query suffice? If it's a machine learning experiment,
you'll likely want to access the data often, in order to try out
different models and hyperparameters etc.

# 2. How much data do you need?

The second thing to think about is the quantity of data you need to
solve the problem at hand. It's tempting to just go ahead and use all
of it. More data is always better, right? Not if you don't need it
all, and not if it makes you slower.

It's very rare that you need _all_ the data you have available. The
obvious thing is to consider only the tables you need for the problem
at hand. How big are they? Big data tools such as Hive are used
because some of the tables are very big, but there's often also a lot
of small tables stored alongside. If you only need small tables you
don't actually have a big data problem.

The second thing to consider is sampling the data. If you are running
an experiment, think about the amount of data that will give you
significant results.

Think about different ways you can reduce the dataset size. It may be
that simple random sampling of the data is not appropriate, for
example in collaborative filtering problems. Instead you could
consider whether it's appropriate to randomly sample _users_ in your
dataset and restrict the dataset to that set of users.

Also consider how much data you need to train a good quality
model. Using a fixed test set, increase the size of the training set
and look at how the metric you care about varies. You may find it
tails off quite quickly, in which case you know how much data you
need.

# 3. Do you have a "needle in a haystack" problem?

If your dataset is very biased, it may make sense to subsample the
majority class. Normally it is enough to do this on just the training
set, since prediction is normally not as costly as training. If you do
need to do it on the test set, be sure you can estimate what the
metrics you care about would be like on the unbalanced data.

# 4. How will you access the data?

For some problems, a single pass through the data is enough. For
others, you will need to read the data repeatedly, or access it in a
random order.

# 5. Where is the data stored?

Moving big data around is slow, so where it's stored becomes
important. The best place to have data is in memory because it makes
everything fast. If you can reduce your data to a size that fits in
memory, you're golden. Write a preprocessing job to get your data into
a local file that you can quickly load into memory.

In my experience it's quite rare that you need more data than fits in
memory. When you do, there are several things you can do.

* If your data is small enough to fit on a regular hard disk,
  i.e. less than a few terabytes, then it might be worth copying it
  locally from wherever it is stored. Transfering data is slow and
  expensive. If you need to read it multiple times then you can save
  hours by copying it and working locally.
* Consider putting your data into a local database, for example
  SQLite, if you need more than simple sequential access to the
  data. With the right indexes, running queries against this database
  will be orders of magnitude faster than querying a big data store
  such as Hive.
* If your data is in a big data store such as Hive (or especially if
  it's in a good one like Google BigQuery or Amazon Redshift), then
  consider leaving the data there. This especially makes sense if you
  are just running a few one off analysis queries or retrieving data
  for visualisation, rather than running a series of experiments. The
  additional engineering time to extract the data locally may well not
  be worthwhile.

# Tricks for big data ML

There have been a few times when I have actually needed to train using
a lot of data. Here are some things I learnt:

* Don't use Spark ML - it is normally orders of magnitude slower than
  Scikit learn and the algorithms are also generally sub-optimal -
  your results will be worse.
* The one exception to this is Spark's ALS implementation, which is
  just very slow, but actually good quality. The best alternative is
  [Ben Frederickson's excellent implicit ilbrary](https://github.com/benfred/implicit).
  This is generally orders of magnitude faster, but unfortunately
  doesn't implement weighted regularization, so the quality is
  sometimes marginally worse.
* If you need to use distributed random forests, you can implement it
  quite easily yourself using Spark together with Scikit-learn's
  decision tree implementation. That is, distribute random samples of
  the data and train a decision tree on each sample in parallel. This
  is much faster and better quality than Spark's decision tree
  implementation.
* For topic modelling, the [Gensim library](https://radimrehurek.com/gensim/)
  is very good at building models incrementally without loading
  everything into memory.

# Finally

Don't forget: tricks and tools for big data are fun - but most of the
time they are not necessary. Don't waste your time if what you care
about is results. And you should care about results.

_(Want to discuss your own specific data problems? Book a [free consultation]({{ site.consultation_url }}) with us -- we're here to help!)_
{% include post_footer.html %}
