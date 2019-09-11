---
title: "Get the most value from your data scientist"
author: Iskander Yusof
excerpt: "Turn your shiny data into shiny gold."
header:
  overlay_image: /assets/images/header-pastry-6.jpg
  overlay_filter: 0.7
---
Most data scientists [don’t generate quantifiable business value]({{ site.baseurl }}{% post_url 2019-08-18-what-data-scientists-actually-do-all-day %}#what-data-scientists-actually-do). You can easily test this for yourself by asking a couple of data scientists about the projects they’ve worked on.

Ask about the impact of their work. You’ll typically hear proud statements such as “I improved the F1 score by 30%” or “I achieved an area under the ROC curve of 0.89”.

This is great! But now ask how exactly these data science-specific numbers relate to an impact on actual business metrics. This is where the conversation starts getting a little fuzzy.

Very few data scientists can honestly say that they’re responsible for a 20% reduction in churn or a 15% improvement in user engagement. At best you might get a hand-wavy explanation of how their work relates to high-level business metrics but they’ll struggle to quantify their impact in a statistically rigorous manner.

But hang on: aren’t data scientists comfortable with numbers? Shouldn’t they have a way to measure the impact of their work? Well, of course they _should_, but this isn’t necessarily their fault.

If it doesn’t even cross the mind of a data scientist to measure business value, then yes, they’re at least partly responsible.

In most cases, though, they _will_ be aware of the problem but they work in a company whose structure makes it impossible for them to generate (and measure) real business value.

And let’s not be too harsh. Measuring and attributing business value correctly is not trivial! It shouldn’t be a huge surprise that you can’t hire a data scientist and magically get a 50% increase in profit.

The goal of this article is to show you how to actually get value from your data scientist. This is in everyone’s interest. Data scientists like it if the work they’re doing has real impact, and you yourself won’t want to have expensive data scientists on your payroll who don’t actually do anything useful.

_Most of this article is written with the assumption that you’ve hired just one experienced data scientist. But the same advice applies to teams as well._

_We’re also assuming that the data scientist is your ~~minion~~ direct report._

## Onboarding your data scientist

Getting the most out of your data scientist starts from the first day of their employment.

You should start by giving them some high-level context: tell them about the business domain(s) they’re expected to help out in and roughly how you’d like to use your data.

Hopefully you’ll already have discussed some of this during the interview stage!

### Putting the data into data science

Obviously you’ll need to tell your data scientist what data you actually have and how it can be accessed.

This sounds straightforward but often you won’t have detailed knowledge of what exactly you have, the quality of the data will be questionable and -- especially in larger companies -- you might even struggle to convince the data owners to grant you access.

The worst-case scenario is that you’re not even in a position where a data scientist can help you, but of course you did [read our other article]({{ site.baseurl }}{% post_url 2019-08-19-are-you-ready-for-data-science %}) so you won’t have made that mistake…

Sometimes you’ll have the right data but the data scientist will have to do some work to make it usable for their purposes. If you’ve [hired the right person]({{ site.baseurl }}{% post_url 2019-08-05-how-to-hire-a-data-scientist %}), they won’t complain about having to do some non-data science tasks before they get to the fun stuff.

In truth, I often like doing basic data engineering tasks myself as I can then be confident that the data ends up in the shape I want (and if it doesn’t, then I’ll only have myself to blame). I’ll also learn a bunch of useful stuff about the data itself in this process.

### Yes to communication, no to silos

Making sure data scientists have easy access to people they’ll need to speak to should be a no-brainer but happens surprisingly rarely.

Introduce your data scientist to the team members they’ll likely need to work with on a daily basis and try to make sure they’re seated in close proximity to these people.

If this isn’t possible (e.g. you have a distributed team), at least ensure it’s not a huge hassle for your data scientist to reach out to their main points of contact. You won’t want your data scientist sitting on their own in a silo.

Also, don’t assume that because data scientists are highly technical, they won’t know how to talk to people in a nontechnical way. Unlike software engineers, we’re not all social outcasts (some of us even _like_ people).

A data scientist should have no problem switching between a technical discussion with a programmer and a conversation with a senior executive who has a completely different mindset. This is why it’s particularly important to test nontechnical communication skills during the [interview]({{ site.baseurl }}{% post_url 2019-08-06-what-should-a-data-scientist-know %}).
{% include post_promo.html %}
### Micromanagement

If you’ve hired only one data scientist, they _should_ be experienced. You shouldn’t need to dictate to them exactly what they need to be doing from day to day.

Give them the broad outlines of your problem and they should be able to work with you to make the problem precise and solvable using data science.

Let your data scientist take the lead on how to solve your problem, but help them out regarding the business context and by facilitating access to the resources they need (in terms of data, tools and people).

<figure>
	<a href="{{ site.baseurl }}/assets/images/venn.png"><img src="{{ site.baseurl }}/assets/images/venn-small.png" alt="Managing a data scientist: who does what?"></a>
	<figcaption>How to divide responsibilities with your data scientist.</figcaption>
</figure>

**Your job is to be a facilitator, not a dictator.**

I can’t count the number of times I’ve been told exactly _how_ to solve a data science problem by a nontechnical person.

This is usually an incredibly bad idea: unless you yourself are a skilled data scientist, it’s very unlikely that you’ll have an idea of the optimal approach.

What’s more, many data scientists won’t have the confidence to push back against what you suggest, so you’ll send them down the wrong path right from the word “go”.

This is a waste of everyone’s time and your money.

Of course, you should still put forward any ideas you have, but be very conscious of how they might be perceived. You should really prioritise describing the problem rather than suggesting possible solutions.

It'll help if you ask your data scientist to propose a solution _before_ you offer some suggestions of your own. For the most part, you should defer to your data scientist regarding what they say needs to be done to solve your data problems.

If you don’t trust them to do this, you’re basically admitting that you made a bad hire!

### Success metrics

Perhaps the most important part of onboarding is to agree on one or more metrics that your data scientist is responsible for improving.

This is a huge topic that deserves its own article, but the first step is simply to tell your data scientist what metrics matter to the business as a whole. This will help frame a discussion of which metrics they’ll be able to improve.

Most likely you’ll have an idea of which metrics you believe your data scientist can help with, but they might be able to move the needle on other metrics as well. So it’s worth letting them know about all the metrics of interest to the business.

**Be realistic:** in many situations, your data scientist won’t be able to optimise for metrics such as revenue or retention directly.

Instead, you’ll want metrics that are fairly narrowly-defined and easy to measure, but [plausibly correlated with business value]({{ site.baseurl }}{% post_url 2019-08-19-are-you-ready-for-data-science %}#metrics-and-business-value).

Also, keep in mind that less is often more: it can be very difficult to move the needle, so ideally your data scientist won’t be working to optimise more than one metric at a time. 

A good outcome from onboarding is an initial [MVP](https://en.wikipedia.org/wiki/Minimum_viable_product) project for your data scientist to get stuck into. Discuss with them what knowledge and resources they’ll need to complete this project in terms of data, tools, people and metrics.

Once they’ve completed their first project, you’ll both have a much better understanding of what they can contribute to your business and can take things from there.

_(In Parts [2]({{ site.baseurl }}{% post_url 2019-08-08-what-your-data-scientist-should-be-doing %}) and [3]({{ site.baseurl }}{% post_url 2019-08-09-how-to-successfully-deliver-a-data-science-project %}) of this series, I'll talk about what your data scientist **should** be doing from day to day in order to deliver value. I'll also explain how to successfully deliver your data science projects._

_Want to discuss your own specific data problems? Book a [free consultation](https://calendly.com/isk-pastry/consult) with us -- we're here to help!)_
{% include post_footer.html %}
