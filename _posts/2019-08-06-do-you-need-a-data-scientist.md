---
title: "Do you really need a data scientist?"
---
I have a confession to make. I hardly ever do data science.

This might sound like a bizarre claim, seeing as almost every job I’ve ever had has the words “Data Scientist” somewhere in its title.

_(Aside: “What exactly do I mean by “data science work”?_

_Well, the term is somewhat ill-defined but I usually use it to mean “something to do with machine learning”. This might include a healthy dose of data cleaning and feature engineering work in addition to model building itself.)_

So what’s going on? Am I getting paid a lot of money to watch YouTube videos of kittens all day long? No, of course not! I only spend 60% of my day on YouTube and most of the videos I watch are about other animals.

But let’s be serious for a few seconds.

As a principal/lead/generally quite awesome data scientist, I receive a lot of requests for help with data science. Typically the conversation goes something like this:

Me: “HELLO I’M ISKANDER HOW MAY I HELP YOU!!!”

Hiring manager: “Er, hello there. Can you turn your mike down a bit?”

Me: “Oh, sorry. How may I help you?”

HM: “No worries. So we need someone who knows a lot about machine learning, and your background and experience sound like they’d be a great fit.”

Me: “Thanks, that’s nice to hear. Can you tell me a bit about your company?”

HM: “So we sell dragon food online. We’ve been in business for three years now and have been growing rapidly. Currently we sell tens of thousands of items a day.”

Me: “Sounds promising, I’ve actually been thinking of buying a dragon myself and I can see how this would be a good business. What would you like me to help with?”

HM: “Well, we’ve got a lot of data on our customers but have never really had the time to look into any of it properly. What we’d like you to do is look into it deeply and tell us what you can find.”

Me: “Cool. Did you have any specific use cases in mind, or would you like me to help you define these as well?”

HM: “We do have a couple of things in mind...”

_At this point I listen closely. I know that the first thing the HM mentions is likely to also be the highest-priority item for them, and hence the reason for the call._

HM (continues): “The most profitable area of business for us isn’t actually dragon food -- it’s the dragon training service we provide our customers.

As you know, dragons are very much _en vogue_ now, but they have the unfortunate tendency to eat their owners. So we help customers train their dragons and reduce the likelihood of their getting eaten to less than 5%.”

Me: “Ah, I understand. So you want me to help you upsell customers to the dragon training service.”

HM: “Exactly! I can see why they call you a genius.”

Me: “Stop, you’re killing me. Can we talk about a few specifics? It sounds like you want me to figure out which customers are likely to purchase your dragon training service.

Based on this, you’d be able to run marketing campaigns to acquire more customers like this, or even personalise your website so that **_DRAGON TRAINING SERVICE!!!_** pops up at exactly the right time for the right customer (unintrusively, of course).”

HM: “Yes!”

Me: “Right, so a good way to start might be to look at your existing customers and seeing which ones have bought the dragon training service, and then we can build a predictive model from there.

Can I ask how many customers typically purchase the service at the moment?”

HM: “That’s actually tricky to answer. You see, the sale doesn’t actually happen online. Because it’s quite an expensive service, we feel it’s better to have one of our dragon trainers make the sale in person.

So the sale itself is entered into our CRM, but often there’s quite a large delay between the sale actually being made and it actually getting logged into our system. The CRM itself is a terrible homegrown system and nobody likes to use it.”

Me: “I see. But it sounds like you should at least have a rough idea of sales figures, even if they’re not exactly up-to-date?”

HM: “Sure, it’s usually somewhere between 5 and 30 sales a month, depending on what campaigns are running.”

Me: “OK. That’s quite a small number of sales, and I can tell you straight away that it might be tricky to train a useful machine learning model on such a small number of positives.

Has anyone looked at the profiles of existing purchasers manually, just to get a general feel for what kinds of buyers you currently have? Perhaps just by talking to them if nothing else?”

HM: “No, as I said nobody has had time to look at the data closely. That’s why we need a data scientist to really look into this more deeply.”

Me: “Ah, OK. Well, perhaps there’s another way we can look at this. Presumably the website functions as a lead generator of sorts, and then you have a dragon trainer who takes the lead and tries to make the sale.”

HM: “That’s pretty much it, yes.”

Me: “Right, it’s not ideal but we could view this as optimising two separate pieces. One is to maximise the number of leads generated by the website, and the other is to maximise the probability of a lead converting into a sale.

Do you know how many leads you’re currently generating from the website?”

HM: “Yes, it’s a few thousand per month.”

Me: “Really? That sounds like a very low conversion rate, so it sounds like you either have a problem with the quality of leads or the follow-up needs to be improved?”

HM: “That is true, but the number of leads is one of the top KPIs for the website, so we’re trying to keep it as high as possible.”

Me: “Wouldn’t it make more sense to have the eventual number of dragon training sales be the KPI? You have to be careful with simply optimising the number of leads as you might end up with a lot of badly-converting leads.”

HM: “The sales data is in the CRM so we can’t track it as easily.”

Me: “Hmm, so it sounds like the first step is to fix this KPI as we need to make sure we’re optimising for something sensible. You’ve mentioned that you have a CRM and presumably you also track visitor behaviour online?”

HM: “Yes, we use Google Analytics.”

Me: “Right, so in order to help you understand your sales, a data analyst -- because this is what I feel you really need before you hire a data scientist -- will ideally have all the data about each customer in one place.

This is surprisingly difficult to do as it involves tracking customers as they proceed from the online world to the offline, and often this can’t be done retroactively."

HM: "OK..."

Me: "So as a first step, you might want to consider migrating to a better CRM that allows you to easily report your sales numbers and will also help to facilitate this online-to-offline tracking.

Migrations are always tricky and I’m usually hesitant to recommend them, but clearly it’s hurting your business if you’re not even able to do reporting from your CRM. You’ll have to weigh the cost versus benefit of this of course.”

HM: “Thanks a lot, this all makes sense. So if we do proceed with this plan, would you be able to help us with the migration?”

Me: “I’ve done a few of these things before, but I’d suggest hiring a specialist instead as it’s obviously important for you and you don’t want to pay for data science skills that you’re not really using.”

HM: “That’s fine, we really need a data scientist as there’s a lot of scope for AI here as well. I didn’t tell you about the other work that needs to be done, which involves consolidating all our data sources...”

Me: “Erm… all right then. I’ve always wanted to learn more about CRMs.”

In reality, of course, I’d turn down any job where I didn’t think I was able to do a good job.

But weirdly, I’ve ended up “qualified” in a whole range of areas that have absolutely nothing to do with data science. This is because I’ve found myself doing “anything and everything to do with data”, and it’s not always obvious what a specific role will entail until you actually get started.

If I had to describe my working life in four sentences, it would be “I solve problems via any means possible. Usually with data. And I'm not very good at counting.”

I’m pretty happy with this as it makes me an easy hire in most situations, but the fact of the matter remains: I’m a data scientist who doesn’t often do data science.

## What data scientists actually do

Most data scientists are:

a) not doing data science or

b) not doing anything that generates actual business value.

I love doing things backwards, so let’s talk about point b) first.

### Producing business value

The best way to ensure your data scientists produce business value is to hold them accountable for their work.

Have a frank conversation with them about what metrics they intend to optimise, how these metrics are relevant to the business and how they intend to go about improving said metrics.

But make sure your data scientists have the remit to effect change throughout the business and **don’t have them sitting in silos on their own**.

If they come up with something good, your job is to ensure they’re able to put their work into production or change the relevant business processes.

You won’t be on your own: a **good** data scientist should be able to arm you with metrics to help you convince other stakeholders that what they’re doing is worth following through with.

A **great** data scientist can go even further, and will be able to put together a realistic roadmap for productionising their work.

Try to **avoid focusing too much on academic credentials** when looking for a data scientist.

Yes, there are data science problems that are essentially research questions, but these are in the extreme minority. And one of the hallmarks of research problems is that they’re not always solvable, which means there’s a high chance that a research-focused data scientist will produce absolutely nothing.

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

**There’s plenty of value in data. Most of it can be extracted without a data scientist.**

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

If you're not sure what category your data problem falls into, just [book a free consultation](https://calendly.com/isk-pastry/consult) with us and we'll talk it over.

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