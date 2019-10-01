---
title: "How to be a 10x data scientist"
author: Daoud Clarke
excerpt: "Experimenting makes you a data scientist, so do it well."
header:
  overlay_image: /assets/images/header-article.jpg
  overlay_filter: 0.6
---


I'm going to tell you what it takes to be a 10x data scientist. What
is a 10x data scientist? Someone who runs ten times as many
experiments as the average data scientist.

Why experiments? Data scientists do other things too: data munging,
analysis, and writing implementations of machine learning algorithms
for production. But experiments are what defines a data
scientist. That's where the _science_ is, and it is what distinguishes
them from a data analyst or a machine learning engineer.

So to be a great data scientist you have to be great at doing
experiments.

Why 10 times more experiments? You can never guarantee you'll get ten
times better results by being cleverer or faster. But you can run more
experiments. And the more experiments you run, the more likely you are
to get better results, the faster you'll iterate and the faster you'll
learn.

Why do you want to be a 10x data scientist? I don't know. Maybe
because it sounds cool. Maybe because it's fun. Maybe because you'll
have more time to eat pastries. That's up to you.

I'm going to assume that you can run experiments correctly. You're a
data scientist, right? Nevertheless, there's one thing I've seen many
data scientists get wrong. It's this:


# 1. Measure your uncertainty

What's the point in improving 5% over the baseline if you don't know
whether the result is statistically significant? Data scientists know
(or _should_ know) statistics, but they are often too lazy to apply
it to their own work.

There is no shortage of options for this. My favourite method is one I
learnt in my physics degree: estimate the uncertainty as the [standard
error in the mean](https://en.wikipedia.org/wiki/Standard_error). Of
course this means that the value you report has to be the mean of
something, whether it's the mean F1 score on five folds in cross
validation, or whether it's the mean precision at 10 over rankings for
1,000 different queries.

You don't need to do statistical significance tests between all your
results. But you need to have a handle on how uncertain your results
are. The standard error in the mean gives you that - if your results
are separated by more than three times the standard error, chances are
the difference is significant.

You probably also want to consider what [effect
size](https://en.wikipedia.org/wiki/Effect_size) you're looking
for. If a 0.1% improvement isn't useful to you then there's no point
in running experiments that can detect this sort of change.


# 2. Big data is not cool

Big data is slow. You don't want to be slow. So use small data. Most
of the time you don't _need_ big data. If you think you need it, spend
a bit of time rethinking to make sure you really do.

You want your dataset to be big enough such that the uncertainty in
your result is _small_ enough to distinguish between differences that
you care about. You don't want it to be any bigger: that's just a
waste of time.

You don't have to use all the data you have available. Depending on
your experiment, you may be able to estimate how much data you
need. Otherwise, look at how the metric you care about varies with
training set size. If it levels off fairly quickly, you'll know you
can get away with discarding a lot of data. Do more experiments to
figure out how much data you need to make the uncertainty low enough
for the insights you're looking for.

The number one cause of slow experiments is using too much data. Just
don't do it.


# 3. Don't use big data tools

If you have small data, you don't need big data tools. Don't use
Spark, it will be horribly slow and the results will be poor compared
to something like Pandas and Scikit-learn. Use that instead.


# 4. Use a good IDE

Use a decent integrated development environment like
[PyCharm](https://www.jetbrains.com/pycharm/) - actually, just use
PyCharm, nothing really compares. Learn how to use it properly.

These are the things that I find most useful:
 - Autocompletion, especially in combination with typed code
 - Viewing parameters and documentation for a function or class
 - Quickly search the whole codebase for a file, class or function
 - Refactor to extract a variable, function or method, and inline variables

I can't bear watching people struggle with a text editor for this kind
of thing. Please stop.

Jupyter notebooks are ok for exploratory work, but if you want to be a
10x data scientist, you need to use an IDE for experiments.


# 5. Cache intermediate steps

An experiment can include preprocessing the data, extracting features,
feature selection and so on. Each of these steps takes time to
run. The chances are, once you've found a good set of features, you
will keep them more or less fixed while you experiment with models. If
the preprocessing step takes a long time, it makes sense to cache the
intermediate steps so that you perform these costly computations just
once. This can make a huge difference to how long it takes to run
experiments.

I will typically do this with one or more preprocessing scripts that
generate files to be used by later stages. Make sure that you keep
track of how these files relate to the source data so that you can
track your experiment results back to the original data, either
through file naming conventions, or a tool designed for the job such
as [Pachyderm](https://www.pachyderm.io/).


# 6. Optimise your code

If your experiment is still slow when you've reduced your dataset
size, then you may benefit from optimising your code. Balance running
experiments with optimising your code while experiments are running.

You should know the basics of how to optimise code. Here's the basics:
use a profiler. The profiler will tell you which bits are slow. Change
those bits until they aren't slow any more. Then run the profiler and
find other bits that are slow. Repeat.

Run the profiler on a small sample so that you can quickly find out
which bits are slow. (You need to optimise the optimising too.)


# 7. Keep track of your results

If you lose the results of your experiments it's a waste. So keep
careful track. Use a tool designed for the job like
[MLFlow](https://mlflow.org/),
[Sacred](https://github.com/IDSIA/sacred), or my own pet project,
[PyPastry](https://github.com/datapastry/pypastry). If you're copying
results around you're wasting time and likely to make errors. Don't.

If you do all the above things, running an experiment will likely take
less than five minutes, ideally less than two. That's long enough to
think about what the next experiment will be.

This means you can potentially run hundreds of experiments in a
day. When you're running that many experiments you need a good way to
keep track.


# 7a. Eat lots of pastries

This one isn't actually good advice. Your brain needs up to 400
calories worth of glucose per day, but eating pastries may not be the
healthiest option to achieve this. But it would be tasty.

Instead you could consider contacting
[DataPastry](https://datapastry.com), the data science consultancy I
run with my cofounder Iskander. If you'd like any advice or need help
with a data science project, [we'd love to hear from
you](mailto:hello@datapastry.com) and we don't bite (except for
pastries).


# Conclusion

If you do all the above things I'm pretty sure you will run at least
ten times as many experiments as the data scientist sitting next to
you (unless you're sitting next to me). Most data scientists don't do
any of them. So if you do them all, you'll probably run fifty times
more experiments. Does this make you fifty times more valuable? I
don't know, but it can't hurt. And you'll have more time for eating
pastries.

_(Want to discuss your own specific data problems? Book a [free consultation]({{ site.consultation_url }}) with us -- we're here to help!)_
{% include post_footer.html %}