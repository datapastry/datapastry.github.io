---
title: "Do you really need a data scientist? _(Part 2/3)_"
author: Iskander Yusof
excerpt: "What do data scientists actually do all day?"
---

_(Continued from [Part 1]({{ site.baseurl }}{% post_url 2019-08-06-do-you-need-a-data-scientist-part-1 %}), where I admitted that I rarely do data science. Scandalous!)_

## What data scientists actually do

Most data scientists are:

a) not doing data science

or

b) not doing anything that generates actual business value.

I love doing things backwards, so let’s talk about point b) first.

### Producing business value

The best way to ensure your data scientists produce business value is to hold them accountable for their work.

Have a frank conversation with them about what metrics they intend to optimise, how these metrics are relevant to the business and how they intend to go about improving said metrics.

But make sure your data scientists have the remit to effect change throughout the business and **don’t have them sitting in silos on their own**.

If they come up with something good, your job is to ensure they’re able to put their work into production or change the relevant business processes.

You won’t be on your own: a _good_ data scientist should be able to arm you with metrics to help you convince other stakeholders that what they’re doing is worth following through with.

A _great_ data scientist can go even further and will be able to put together a realistic roadmap for productionising their work.

You should also avoid focusing too much on academic credentials when looking for a data scientist.

Yes, there are data science problems that are essentially research questions, but these are in the extreme minority.

And one of the hallmarks of research problems is that they’re not always solvable, which means there’s a high chance that a research-focused data scientist will produce absolutely nothing.

I’ve worked in a few data science teams that felt like an attempt to replicate academia in industry, with a bigger focus on publishing papers than producing anything useful for the business.

Admittedly this can be great fun and it’s important for data scientists to stay in touch with cutting-edge research, but unless you’re Google or Microsoft you probably can’t afford to have this be the sole focus of any data scientist you hire.

### Data scientists who don’t do data science

You’ll find many “data scientists” who are actually doing the work of a data analyst, a data engineer or a software engineer (oh dear). In this case, they’re generating value for you but they’re not doing “data science”.

But what’s in a name? Does the job title matter as long as they’re useful?

Well, the problem is that they usually won’t be anywhere near as good as an actual specialist in the field, so your data reporting/engineering/architecture will now be half-baked compared to what you’d be getting if you’d hired the right person in the first place.

Also, your “data scientist” likely won’t want to work for you for much longer if they’re actually interested in doing real data science -- and most data scientists are.

There’s a fair chance that they’re quite junior (you didn’t just hire them because they were cheap, did you?) and simply using your company as a stepping stone for a real data science job, most of which require at least 1-2 years of industry experience.

Of course, not having an employee stick around for 300 years isn’t necessarily a problem, but you’d probably prefer someone who would actually enjoy the job and stay with you for a bit longer.

Sometimes it does make sense to hire a data scientist to be your “everything data” guy even if only 10% of what they do is data science. This is especially true in startups where it’s normal for employees to wear multiple hats. 

It’s probably fair to say that if you _do_ need an “everything data” guy, then a well-rounded data scientist is a pretty good bet. An experienced data scientist can often do the occasional data analytics or engineering task but the reverse is very difficult.

Think about your top data-related priorities and ask yourself where data science sits in the hierarchy: if your main requirements are reporting aggregate metrics and getting a better understanding of your data, then a good data analyst should be just fine.

Don’t kid yourself about what you actually need, and make sure any data professional you hire knows what type of work to expect.

### If data scientists aren’t doing data science, what _are_ they doing?

Wait, isn’t this the same as the previous section? Well, kind of, but there are a few common problems I wanted to point out explicitly, namely:

*   Your data exists in many different places and your data scientist will spend their entire working life getting it into one place and then doing basic reporting on the data.
*   You don’t have enough data to justify the use of machine learning, and a good software engineer applying simple heuristics would do the job at least as well.
*   Most of the value in your data can easily be extracted without needing to hire a ludicrously-overqualified data scientist to apply the latest and greatest techniques.

None of this is meant to imply that data scientists shouldn’t have any knowledge of areas outside machine learning.

In fact, the opposite is true: ideally a data scientist should at least have a basic understanding of sister areas such as data warehousing and software engineering.

And if your data scientist is going to be building a predictive model, it usually makes sense for them to perform the relevant data munging and cleaning tasks themselves.

The crucial distinction is that when a data scientist does non-data science work, this should be simply be support for a real data science task. If the task as a whole doesn’t involve data science at all, then you’ve given the job to the wrong person.

## Data science: it’s not magic

Why are so many data scientists hired if they’re not really needed? My opinion is that this is due to two interrelated reasons: one is fear of missing out (FOMO), and the other is simply ignorance of what a data scientist can and can’t do.

_(Aside: To a large extent, unnecessary hiring isn’t unique to data science._

_Especially in large companies, I’ve often encountered employees where I’ve felt “Hmm, this person’s job is not really necessary. Almost everything they do is busywork.” But hopefully you want to run a more efficient operation than that.)_

Let’s talk about FOMO first.

Unless you’ve been living under a rock the size of a planet, you cannot fail to have heard the hype around “the AI revolution”, “automation”, “the robots are coming to take our jobs” and other bombastic claims made by people who don’t actually work in the field.

So naturally you might feel like unless you embrace the AI revolution yourself, your company will go the way of the dinosaur, and you definitely don’t want that. Who can help you get on the bandwagon? How about an **AI expert**!

And what are **AI experts** usually called? Well, “data scientists” for one…

Hopefully you’ll agree that FOMO is not a good thing to base a company’s hiring decisions on. So let’s now talk about the second, more concrete factor.

What can data scientists actually bring to the table? Very broadly, data scientists extract value from data. Slightly more precisely, data scientists find patterns in data and then exploit these patterns to predict things you care about based on past events.

To find these patterns, the data scientist will need data (duh!). What kind of data will they need?

Well, imagine that you’re a homeowner and you want to predict the sale price of your property, which is just another way of saying you want to value your property. Naturally, this would be based on a range of different factors including the property’s location, size, condition and so on.

You’d then want to relate these factors to the property price. The more historical data you have connecting a property’s price to its location, size and condition, the easier it will be to value your own property. 

Data scientists basically do the same thing as you do when you value a property, except in an automated fashion and on a larger scale.

And just like you, they’re most effective when they have (or are able to generate) lots of high-quality data that is strongly related to the thing they’re trying to predict. **Without good data, a data scientist is less valuable than an inedible pastry.**

You might hope that a data scientist will be able to use machine learning to find patterns that a human would never be able to. In a way this is true, because they can write code to look at far more data than a human could.

**But don’t expect to see something magical.** Typically data scientists will find patterns that are fairly intuitive, except that they’ll be able to tell you _exactly_ how a property’s price relates to its location and size and when this relationship doesn’t hold up.

It’s also common for data scientists to _invalidate_ a lot of prior assumptions and conventional wisdom in a company. Being truly data-driven means you’ll listen to them when they tell you that your intuition about what kinds of customers are most likely to churn was completely wrong.

What about getting “insights” from data? Sometimes data scientists will do clever things to generate pretty pictures so they can say things like “oh look! Most of our customers fall into one of these seven big clusters.”

What do they do with these clusters? Usually not very much, but for a brief time it will look like they’ve done something important. (This kind of clustering _can_ be useful, but all too often it is used simply to generate attractive visualisations without much tangible value.)

**If you only want to understand your data better, hire a good data analyst.**

They’ll know how to interrogate your data using SQL and other tools to pull out the numbers you care about, as well as how to present these numbers in an easy-to-digest format for other stakeholders. They can even generate pretty pictures!

And then you can hire a data scientist once you actually need to predict something.

Personally, I love it when I start with a client and they already have a data analyst working there, because I can then be confident that someone actually understands the data and has made an effort to ensure it’s usable.

Working with hitherto-untouched data is like eating a random object that a stranger has handed to you: there’s a small chance that it’ll be a delicious pastry, but it’s a lot more likely that you’ll get food poisoning.

There’s plenty of value in data. Most of it can be extracted without a data scientist.

_(In the [final part]({{ site.baseurl }}{% post_url 2019-08-06-do-you-need-a-data-scientist-part-3 %}) of this series, I'll say more about when you **should** and **shouldn't** hire a data scientist._

_Want to discuss your own specific data problems? Book a [free consultation](https://calendly.com/isk-pastry/consult) with us -- we're here to help!)_