---
title: "Are you ready for data science?"
author: Iskander Yusof
excerpt: "Probably not. But here's how to find out."
header:
  overlay_image: /assets/images/header-pastry-3.jpg
  overlay_filter: 0.6
---

_(Continued from Parts [1]({{ site.baseurl }}{% post_url 2019-08-17-you-dont-need-a-data-scientist %}) and [2]({{ site.baseurl }}{% post_url 2019-08-18-what-data-scientists-actually-do-all-day %}), where I explained why data scientists are usually a waste of time and money.)_

## When _shouldn’t_ you hire a data scientist?

Let’s highlight a couple of common data problems faced by companies for which a data scientist shouldn’t be necessary.

**Problem:** You have a reasonably clean customer database but don’t really understand your customers. Basic questions like “where do our customers live?” are hard to answer.

**What you actually need:** A data analyst who specialises in reporting and visualisation.

Part of this will involve creating a consistent set of metrics across the company that all stakeholders agree on, so you’ll need someone who has a good understanding of business as well as raw analytical skills.

**Problem:** Your data is easily-accessible but is very messy. The prospect of having to actually work with the data fills you with dread.

**What you actually need:** This depends on _why_ you want to clean the data.

Cleaning isn’t a worthy goal in and of itself and you won’t be able to prioritise correctly unless you know what you want to do with the data.

If the main goal is to report aggregate metrics, then hire a data analyst who has sufficient programming skills to clean the data and is happy to maintain documentation for your data.

If the goal is predictive modelling, then yes, consider hiring a data scientist to do this work.

**Problem:** Your company is in an industry that isn’t particularly technically sophisticated.

You do have many data sources and think there would be a lot of value in getting all this data into a data warehouse as a single source of truth, as well as to give a complete view of each customer and your business as a whole.

**What you actually need:** This is a complex task for which you’ll most likely want to make multiple hires.

At the very least you’ll need a data architect to make technical decisions regarding how to get all data sources into one place, as well as a data governance manager to ensure a consistent level of quality is maintained across all sources.

Again, simply getting all data into a data warehouse isn’t by itself a sensible goal, so consider making hiring decisions based on the actual problems you want to solve using your data warehouse.

Consider developing an [MVP](https://en.wikipedia.org/wiki/Minimum_viable_product) first. You might initially be able to extract a lot of value by just getting two sources of customer data into a single place, e.g. by merging website analytics data with marketing campaign data.

You'll also want the "consumer" of the data sources to be happy with the outcome, which means you might need a data analyst or data scientist to specify their use cases to the data architect.

**Problem:** You’re generating huge quantities of sensor data every second and need someone to architect a system to ingest and process this data.

**What you actually need:** A data engineer. Presumably you have a reason for wanting this data (see the theme here?), so make sure the work the data engineer does is in service of this goal.

If you need this data for predictive analytics, you might also want the advice of a data scientist to help inform some of the data engineer’s decisions.

------

Unfortunately there’s often no connection between a job’s title and its actual responsibilities -- which is part of the reason this article exists!

For this reason, “data analyst” is the answer to a lot of these questions, but the specific flavour of data analyst you should hire varies a lot.

There’s a big difference between a data analyst who can produce visualisations for C-level executives using Tableau and a data analyst who can knock your data into good shape.

You might prefer to use more specific titles such as “data quality analyst” when looking for a new hire. Sometimes you’ll get lucky and find all the skills you might conceivably need in a single person, but if not, you should identify your top priorities and aim to hire for those.

## When _should_ you hire a data scientist?

Only consider hiring a data scientist if you’re sure that your current team won’t be able to adequately address your problem.

If you have a task that can be expressed as a “prediction problem”, then you’ll probably need a data scientist.

What’s a “prediction problem”? This means you’d like to predict something based on historical data. For example, you might want to:



*   Predict what customers are likely to buy on a website given the purchasing behaviour of similar customers.
*   Figure out what’s most likely to happen in an election based on the outcome of previous elections.
*   Determine how to spend your marketing budget. A data scientist can help you do this by predicting your expected return on investment based on the amount of money you put into each marketing channel.

It won’t always be obvious if your task is a prediction problem.

If you have a business process that involves manually typing up handwritten forms and pushing the entries into a database, then a data scientist could help you automate this process. They would write software that “predicts” (recognises) what has been written in your forms based on historical handwriting data.

If you're not sure what category your data problem falls into, just book a [free consultation](https://calendly.com/isk-pastry/consult) with us and we'll talk it over.

## MVP data science

The concept of an MVP (Minimum Viable Product) is well-known in the startup and technology communities.

Very simply, the idea is to put together the smallest possible product that does something useful, in order to test whether or not the basic idea for the product resonates with the market. The MVP is then improved iteratively based on the feedback from customers.

You can do “MVP data science” in a similar way.

What’s the bare minimum you need for a data scientist to produce something useful? Here’s a checklist showing what is _essential_ and what is _nice to have_ before you call upon the services of a data scientist:



_**Essential**_
*   You have a “prediction problem”. Think carefully about whether the task you have can be described as such.
*   You have some historical data that could plausibly be used to make these predictions.

	Remember: **don’t expect magic**. You’re not going to find a data scientist who can accurately predict a stock price based solely on its historical movements.

_**Nice to have**_
*   Ideally you should know what success looks like. You should have a rough idea of how much business value there is in solving your prediction problem.

	If it potentially means £10m in reduced marketing expenditure, that’s great.

	But if it simply means saving 30 minutes a day, that might only be worth £10,000 and it’d be hard to justify hiring a data scientist.
*   Your data is reasonably easy to access.

	As long as they’ve been granted access, a good data scientist should generally be fine with pulling data from different sources. But things get a lot harder if the data owners are unknown, hard to get hold of, or unconvinced of the merits of your problem.
*   You know roughly what data you have (e.g. in the form of a semi-maintained data dictionary, or at least someone who the data scientist can call upon when they have questions about the data).
*   You have some understanding of high-level metrics related to your prediction problem.

	For example, if you want to reduce churn for your SaaS business, you should ideally know the current churn rate and how this breaks down across different types of customers.
*   You’ve taken “obvious” actions to solve your problem that don’t necessarily involve a data scientist.

	Using the churn example again, there are many simple things you can do to reduce attrition that don’t involve building a predictive model of potential churners.

## Metrics and business value

Let’s close with a topic that everyone pays lip service to but -- in my experience -- is very rarely done well.

That is, what metrics should the data team be optimising for and what business value do you expect them to generate?

Most “obvious” KPIs such as revenue or retention will be too broad to optimise for directly. Almost any individual project will struggle to demonstrate an immediate impact on these KPIs, but clearly this doesn’t mean that all such projects are useless.

Instead, try to come up with metrics that are fairly narrowly-defined and **easy to measure, but plausibly correlated with business value**.

Expect these metrics to evolve our time as your data team matures. Eventually, your data scientists should be able to directly demonstrate what value they have added to the business. 

You can help your data team by making it clear what metrics actually matter for your business and regularly reviewing the data team’s internal metrics to ensure they are aligned with your business goals.

Also, it's fine if your team needs to define a new success metric for a specific project, as long as they are able to justify why it is the right metric to use.

Sometimes your data scientists _will_ be able to actually quantify the relationship between the metrics they’re optimising for and your global business metrics, but often this will be more art than science.

With enough small improvements to your data team’s metrics, you should start to see the effects compounding over time and the needle moving on your main business KPIs.

Don’t underestimate the difficulty of establishing, maintaining and tracking a good set of metrics for your data team. Correctly assessing the impact of any given change requires a lot of statistical rigour and maturity across multiple business units.

And most claims I’ve seen along the lines of “my work led to millions of dollars more in revenue” just don’t hold up once you examine them closely.

Hey, nobody said data science was _easy_.

_(That's it for this article series! Stay tuned for future DataPastry articles: we'll explain how to hire and get the most value from a data scientist._

_If you're of a more technical bent, we'll also talk about how to design your data infrastructure in a way that won't make your data analysts and scientists cry. Spoiler: we think Apache Spark is mostly useless._

_Want to discuss your own specific data problems? Book a [free consultation](https://calendly.com/isk-pastry/consult) with us -- we're here to help!)_
{% include post_footer.html %}