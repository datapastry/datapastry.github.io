---
title: "Get the most value from your data scientist"
---
Most data scientists [don’t generate quantifiable business value](https://drive.google.com/a/datapastry.com/open?id=1nBXCdlWGVigZTlHrx_cntNph-vXl-WLpRVHhPI-lrbU). You can easily test this for yourself by asking a couple of data scientists about the projects they’ve worked on.

Ask about the impact of their work. You’ll typically hear proud statements such as “I improved the F1 score by 30%” or “I achieved an area under the ROC curve of 0.89”.

This is great! But now ask how exactly these data science-specific numbers relate to an impact on actual business metrics. This is where the conversation starts getting a little fuzzy.

Very few data scientists can honestly say that they’re responsible for a 20% reduction in churn or a 15% improvement in user engagement. At best you might get a hand-wavy explanation of how their work relates to high-level business metrics but they’ll struggle to quantify their impact in a statistically rigorous manner.

But hang on: aren’t data scientists comfortable with numbers? Shouldn’t they have a way to measure the impact of their work? Well, of course they _should_, but this isn’t necessarily their fault.

If it doesn’t even cross the mind of a data scientist to measure business value, then yes, they’re at least partly responsible.

In most cases, though, they _will_ be aware of the problem but they work in a company whose structure makes it impossible for them to generate (and measure) real business value.

And let’s not be too harsh. Measuring and attributing business value correctly is not trivial! It shouldn’t be a huge surprise that you can’t hire a data scientist and magically get a 50% increase in profits.

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

The worst-case scenario is that you’re not even in a position where a data scientist can help you, but of course you did [read our other article](https://drive.google.com/a/datapastry.com/open?id=1DvfXuFhdlh0wngcdmfvLdZCeKfodyT43V72YPLFdKvM) so you won’t have made that mistake…

Sometimes you’ll have the right data but the data scientist will have to do some work to make it usable for their purposes. If you’ve [hired the right person](https://drive.google.com/a/datapastry.com/open?id=1R-hkHvkr8vZdXPscrKRBUHE5GTMwnDkQtifbgbtmqos), they won’t complain about the fact that they have to do some non-data science tasks before they get to the fun stuff.

In truth, I often like doing basic data engineering tasks myself as I can then be confident that the data ends up in the shape I want (and if it doesn’t, then I’ll only have myself to blame). I’ll also learn a bunch of useful stuff about the data itself in this process.

### Yes to communication, no to silos

Making sure data scientists have easy access to people they’ll need to speak to should be a no-brainer but happens surprisingly rarely.

Introduce your data scientist to the team members they’ll likely need to work with on a daily basis and try to make sure they’re seated in close proximity to these people.

If this isn’t possible (e.g. if you have a distributed team), at least ensure it’s not a huge hassle for your data scientist to reach out to their main points of contact. You won’t want your data scientist sitting on their own in a silo.

Also, don’t assume that because data scientists are highly technical, they won’t know how to talk to people in a nontechnical way. Unlike software engineers, we’re not all social outcasts (some of us even _like_ people).

A data scientist should have no problem switching between a technical discussion with a programmer and a conversation with a senior executive who has a completely different mindset. This is why it’s particularly important to test nontechnical communication skills during the [interview](https://drive.google.com/a/datapastry.com/open?id=1R-hkHvkr8vZdXPscrKRBUHE5GTMwnDkQtifbgbtmqos).

### Micromanagement

If you’ve hired only one data scientist, they _should_ be experienced and so you shouldn’t need to dictate to them exactly what they need to be doing from day to day.

Give them the broad outlines of your problem and they should be able to work with you to make the problem precise and solvable using data science.

Let your data scientist take the lead on how to solve your problem, but help them out regarding the business context and by facilitating access to the resources they need (in terms of data, tools and people).

I can’t count the number of times I’ve been told exactly _how_ to solve a data science problem by a nontechnical person.

This is usually an incredibly bad idea: unless you yourself are a skilled data scientist, it’s very unlikely that you’ll have an idea of the optimal approach.

What’s more, many data scientists won’t have the confidence to push back against what you suggest, so you’ll send them down the wrong path right from the word “go”.

This is a waste of everyone’s time and your money.

Of course, you should still put forward any ideas you have, but be very conscious of how they might be perceived. You should really prioritise describing the problem rather than suggesting possible solutions.

And ask your data scientist to propose a solution _before_ you offer some suggestions of your own. For the most part, you should defer to your data scientist regarding what they say needs to be done to solve your data problems.

If you don’t trust them to do this, you’re basically admitting that you made a bad hire!

**Remember: your job is to be a facilitator, not a dictator.**

**_<Venn diagram with two circles: your responsibilities vs. data scientist’s responsibilities. For you: setting business context, relaying important business outcomes/KPIs, giving high-level problem definition, facilitating communications, helping with access to tools and data. For data scientist: making problem definition precise, designing and implementing solution, high-frequency/granular communications with relevant team members. For both: championing work for/selling work to other stakeholders, defining success metrics, resourcing (data, tools, people)>_**

### Success metrics

Perhaps the most important part of onboarding is to agree on one or more metrics that your data scientist is responsible for improving.

This is a huge topic that I can’t possibly do justice to here, but the first step is simply to tell your data scientist what metrics matter to the business as a whole. This will help frame a discussion of which metrics they’ll be able to improve.

Most likely you’ll have an idea of which metrics you believe your data scientist can help with, but they might be able to move the needle on other metrics as well. So it’s worth letting them know about all the metrics of interest to the business.

Be realistic: in many situations, your data scientist won’t be able to optimise for metrics such as revenue or retention directly.

Instead, you’ll want metrics that are fairly narrowly-defined and easy to measure, but plausibly correlated with business value. **<link to Metrics and business value in You don’t need a data scientist article>**

Also, keep in mind that less is often more: it can be very difficult to move the needle, so ideally your data scientist won’t be working to optimise more than one metric at a time. 

A good outcome from onboarding is an initial [MVP](https://en.wikipedia.org/wiki/Minimum_viable_product) project for your data scientist to get stuck into. Discuss with them what knowledge and resources they’ll need to complete this project in terms of data, tools, people and metrics.

Once they’ve completed their first project, you’ll both have a much better understanding of what’s possible for your business and can take things from there.

## What to expect from your data scientist

Data scientists excel at solving “prediction problems” where they have to predict something based on historical data.

For example, your data scientist might predict which customers in your subscription business are most likely to leave (“churn”) within the next month.

In this example, three things will need to happen:



1. **Preparation:** Before your data scientist can do any real work, they’ll need to get hold of your data and knock it into a shape where they can do some fancy predictive modelling.
	
	They’ll also need tools to work with the data and ideally should have access to people who can tell them more about the data they’ll be working with.

	Even the smartest data scientist won’t be able to figure out what a field called `xgr671` means without any context.
2. **Prediction:** Your data scientist will need to build a _model_ that predicts which customers are most likely to churn. 
3. **Action:** Your company will take some sort of action based on the model’s predictions.
	
	For example, you might proactively contact customers who are likely to churn and offer them incentives to stay with you.

You’ll find lots of data scientists who are good at building models but relatively poor at knowing what to do with the results. But both the prediction and action steps are essential for you to get any value out of their work.

A good data scientist will have their eye on the whole picture instead of focusing solely on building good predictive models.

### The preparation stage

If your data scientist has access to a large quantity of clean, well-documented historical data on whatever it is you want to predict, then their job will be _much_ easier and they’ll be able to get to the next stage in no time at all.

Yeah, this hardly ever happens in the real world.

In reality, your data is probably a complete mess and the people responsible for data curation left 18 months ago to go backpacking around the world. Good for them!

So let’s hope you hired a resourceful data scientist who is prepared to grind their way through this stage. Their task will be to figure out how to turn your horrible data into something they can use to build a predictive model.

Ultimately, what they’ll look to build is a set of “features” (variables) that might be predictive of the thing you want to model. This is called _feature engineering_.

Taking the churn example as an example (ha), you might expect churn to be influenced by features such as the length of time a person has been a customer, how much they’ve used your service recently, how often they’ve left you positive feedback and so on.

There’ll normally be many other factors where you have no idea if they have an impact on churn, such as seasonality or the age of the customer.

Your data scientist will prioritise the features that are “obviously” important but also try to include other features that may or may not matter, depending on how much time and effort it takes to do so.

Their magic machine learning model will be the final arbiter of which features are actually relevant, so it usually makes sense to feed it with as much data as possible.

Needless to say, **domain knowledge is extremely valuable** for engineering good, predictive features.

Your data scientist won’t necessarily have any domain knowledge. I used to work in drug discovery where I initially had no idea what features might be predictive (as I was neither a medicinal chemist nor a drug dealer).

To help your data scientist come up with good features, make sure they have access to someone who can tell them more about the specific domain they’re working in. It’s very possible that this “someone” might be you!

When all is said and done, your data scientist will have expended a lot of blood, sweat and tears to construct a big table with one row for each customer showing whether they churned and their corresponding feature values.

This is what they will use to build a machine learning model to predict churn. Hopefully their model will be awesome. But it’s also possible that their model will be rubbish.

**_include example table for churn_**

### The prediction stage

In the churn example, you should expect that your data scientist will build a model that gives you an idea of who is most likely to churn.

By testing the model predictions on data it has never seen before, your data scientist should also have an idea of how accurate the model is. This is called “offline evaluation” (as opposed to “online evaluation”, where the model is tested after it has gone live).

Most likely the model won’t be perfectly accurate with its predictions, so you’ll need to discuss with your data scientist how much accuracy you need for it to be useful.

For many use cases you can still get a lot of utility out of a predictive model that is only slightly better than random guessing. On the other end of the spectrum, there are some problems for which you’ll require a very high level of accuracy.

To decide which category your problem falls into, your data scientist will need to work backwards from your definition of “success” and determine how much accuracy the predictive model needs to achieve this.

(Don’t forget that you should have defined this success metric during onboarding!)

It might indeed turn out that you don’t need an extremely accurate model to achieve what you want.

There are also dozens of metrics for assessing the accuracy of a machine learning model. It’s your data scientist’s responsibility to figure out which metric is most suitable for your problem.

Try to ensure they give you at least a cartoon explanation of whatever metric they decide on. Also, don’t forget that this metric will usually not be the same as the success metric you agreed on during onboarding, although the two metrics should be clearly correlated.

This is super-important to understand, so here’s an example.

You might have defined success as minimising the “percentage of customers who churn in the next month”. And your data scientist’s metric will be aimed at determining how good their machine learning model is at finding out _which_ customers will churn.

But simply identifying these customers isn’t the same as preventing them from churning. To achieve your goal of reducing churn, you’ll need to take an action based on this knowledge.

The outcome of the data science project will depend on both the accuracy of the machine learning model _and_ how successful you are at _acting_ on the model’s insights to encourage customers to stick with your subscription service.

Which leads us nicely to the next step…

### The action stage

Once you’re happy with the model then you’ll need to “productionise” it in some way.

To do this, you’ll need to think about who is the _consumer_ of your data scientist’s work.

Is the machine learning model meant to be a single component of a larger software system, in which case your data scientist will need to collaborate with your software engineers?

Or will your data scientist be creating marketing segments to be used in campaigns run by your lead generation function?

Model productionisation (or “deployment”) is a large topic in its own right but it doesn’t necessarily have to be complex, at least in the first iteration.

Productionisation of your model _might_ need a data engineer but it isn’t always essential.

If you’re just starting out with machine learning then we’d recommend hiring a data scientist who can at least do the basics of model deployment, especially in situations where the data science function isn’t yet mission-critical.

This is particularly true now that deployment in cloud environments like AWS or GCP is easier than ever. You can always hire a data engineer once your data scientist has proved the value of their work and they start hitting the limits of their deployment knowledge.

### Online evaluation

So the outcome of the action stage will be a productionised model that is integrated into your business in some way.

Once your data scientist’s model has gone live, its effectiveness should primarily be judged by your business-focused success metric. And this usually _won’t_ be the data science-specific metric your data scientist came up with in the first stage.

I know, I repeat myself, but this really is very important.

The last thing you want is to be discussing improvements in the Kullback-Leibler divergence (what?) when you really need to be focused on a plain-English metric like “percentage of churners”.

(Incidentally it’s common to monitor all sorts of metrics for a deployed model, including data science-specific metrics, but the purpose of this monitoring is _only_ to ensure everything is running as expected.)

Your data scientist should be responsible for demonstrating that the data science project has actually resulted in an improvement to your success metric.

They should also be able to quantify this improvement. To do this, they might mention “running an A/B test”. Or “multi-armed bandits” if they want to impress you with fancy words.

Regardless of which specific methodology they use, if you’ve hired a good person then they should have a plan for quantifying the improvement (if any) generated by their work.

Bizarrely, I’ve worked in a few places that skip the online evaluation step completely and rely solely on offline metrics to judge the success of their data science efforts.

Believe me, you don’t want to be one of _those_ companies...

### Make your requirements clear

It’s essential that you talk through what you’re planning to do with the model _before_ your data scientist starts doing any real work on your project.

This doesn’t need to be completely set in stone but your plans will have a large influence on the approach the data scientist takes. You don't want a machine learning model that turns out to be useless because you didn’t make it clear to your data scientist what the actual requirements were!

For example, perhaps you’ll need the model to be interpretable, i.e. not a “black box” where you don’t know _why_ it’s making certain predictions.

Or perhaps the model needs to produce predictions in real time. If you’re trying to decide if a credit card transaction is fraudulent then your customers won’t want to wait a long time for the transaction to be processed.

I’m feeling unimaginative so let’s emphasise the point by talking through the churn example yet again.

Imagine that your data scientist builds a machine learning model that seems to be very accurate, and its main insight is that “people who have left the country are likely to churn”.

But if your service only works in one country then you have no chance of convincing someone who is permanently leaving the country to continue using it.

So now you have a new requirement for the churn model: it doesn’t just need to identify customers who are likely to churn, but it also needs to find churn-tastic customers that can _also_ plausibly be convinced to stay.

Now your data scientist will have to actually earn that high salary you’re paying them!

## Minimum viable data science

For your first data science project, your data scientist should ideally work through the entire process from building a machine learning model through to live deployment as quickly as possible (think weeks rather than months).

Avoid the temptation to prematurely optimise any particular aspect of the process. The project as a whole should be viewed as an MVP, i.e. the smallest amount of data science work that will conceivably move the needle on your success metric.

**You don’t need perfection in order to show concrete results.**

Once your data scientist has completed their first MVP, the end-to-end framework for building, deploying and evaluating machine learning models will be in place. They can then build on this and iteratively improve their data science solution over time.

## Empowering your data scientist

To get the most value from a data scientist, you should act as a facilitator for the work they do and make it easy for them to effect change. But what does this actually mean?

### Put your data scientist in the middle

The weird hybrid nature of data science means that we data scientists usually need to communicate with all sorts of people across the company.

At various times data scientists will have to talk to programmers, data engineers, data analysts and design/business/product people.

We strongly suggest that your data scientist work in close collaboration with your programmers and data engineers. Only hire someone you’d trust to be comfortable in this environment and who can put code into production directly.

If you have a data engineer, they should help support your data scientist’s goals and objectives. This means your data scientist will need to regularly communicate what they’re working on to the data engineer.

Again, this _should_ be obvious but I’ve worked in many places where the data scientists’ and data engineers’ respective goals were completely misaligned.

In addition to this, whatever your data scientist is working on will presumably have some kind of commercial impact, so they’ll need to be able to pick the brains of the relevant business/product people.

Usually data scientists don’t need or want daily contact with strange nontechnical folk, but it should still be easy for them to get hold of the people they need when necessary.

Often the work your data scientist is doing will need buy-in from stakeholders in some other business function. (I’ve lost count of the number of times I’ve had to present to people with titles like “Head of Marketing for Blabla”.)

A good data scientist should be able to convince the relevant stakeholders of their project’s business value without needing to resort to jargon. They should also be able to work with other functions to deliver their project without requiring too much in the way of adult supervision.

Last but not least, if you have a data analyst you’ll want them to be seated close to your data scientist. This is a no-brainer as both parties should be able to assist each other a lot; in particular, your data analyst can help onboard your data scientist in the first couple of weeks.

So in summary:

*   Embed your data scientist into your engineering team. If you hired a strong coder then they should be fine in this environment.
*   If you have a data analyst, put them next to your data scientist. It might be a bit scary for an analyst to work next to engineers, but most engineers are only really dangerous if provoked.
*   Facilitate easy communication between your data scientist and the relevant business/product folks.
*   Hire a data scientist who can put on their business hat and convince nontechnical stakeholders of the value of their work.

Incidentally, this team structure doesn’t need to change much if you have multiple data scientists.

You might want to designate one data scientist as a team lead but often this doesn’t make sense, e.g. if each data scientist is highly experienced and has ownership of their own project.

### Tools of the job

You’ve probably heard of the expression “a poor craftsman blames their tools”, but as far as data science is concerned these are _not_ good words to live by.

You should aim to get your data, infrastructure and code into a shape where your data scientist can run experiments quickly in short iterations. At a rough guess, I would say that issues with tooling can decrease your data scientist’s productivity by a factor of up to 5x. 

Even worse, slow experiment cycles will push your data scientist towards using theoretical arguments about what will work best rather than testing their hypotheses empirically.

This is the wrong way to do data science -- mainly because it leads to results that are wrong, period. So **make experimentation easy.**

Of course, tooling will never be perfect and a good data scientist should be able to work around minor problems. But you should listen to your data scientist when they tell you that they’re struggling to get much done due to issues with data, code quality or infrastructure.

Have a frank discussion about the impact of these problems and then prioritise fixes accordingly.

Problems with tooling can range from being a minor irritation to being the root cause of huge delays or major mistakes further down the line, so you’ll want to make sure you tackle these issues _before_ they negatively impact your business.

### Personal goals

Data scientists are people and people usually have their own individual needs and desires. It’s always good to help your data scientist achieve their long- and short-term personal goals.

Selfishly, this is in your interest as the data science market is very hot -- you can expect an experienced data scientist to leave at the first possible opportunity if they’re not happy with what they’re doing.

We suggest that you conduct regular 1-1s with your data scientist to ensure they enjoy the work they’re doing and to allow them to air any concerns they have in private (or more positively, to share any ideas they have).

Of course, this doesn’t mean communication shouldn’t also happen organically, but in a busy work environment it can be easy to overlook the wellbeing of any individual worker drone.

Try to make sure that the work your data scientist is doing is aligned with their own personal goals.

The reality of commercial data science work is that much of a data scientist’s time can be consumed by data wrangling and other tedious tasks. But you can try to mitigate the drudgery by finding work for them that is more intellectually fulfilling.

For example, if your data scientist wants to spend one day a week doing investigative work that isn’t guaranteed to pay off, see if you can make this happen. It’s entirely possible that their research could result in a big win for the business!

Lots of data scientists also like feeling like they’re not isolated from the community at large, which is especially relevant if you only have one data scientist in your company.

If they’re interested, let your data scientist take the time to go to data conferences and meetups. They can also talk about how great your company is for data scientists -- or discourage anyone else from applying if it’s actually a terrible place to work (just kidding, only people in awesome companies read our articles).

## Data science processes

### Agile data science

It’s a slightly controversial point, but I believe _commercial_ data science work can and should obey normal software engineering practices.

In fact, I would argue that the best kind of data scientist is actually a decent software engineer who knows a lot about machine learning and is pretty good at communication.

_(Aside: No, I’m not describing a “unicorn”. Lots of software engineers work in fields such as game development that **also** require advanced domain knowledge and we don’t have special names for them. Why should data science be different?)_

Naturally, this goes hand in hand with the idea of embedding your data scientist into the engineering team.

So this means that your data scientist should participate in sprints and standup meetings like everyone else. Data science projects can and should be broken down into small, clearly-defined tasks with concrete deliverables.

Of course, it can be difficult to scope data science tasks correctly -- it’s hard enough in software engineering! In particular, open-ended investigative work tends to be harder to estimate than coding and data munging.

A smart data scientist should know which tasks have the most uncertainty and work to reduce this as much as possible at an early stage, so estimation quickly becomes a lot more accurate.

In general we’d recommend using timeboxed [spikes](https://en.wikipedia.org/wiki/Spike_(software_development)) to handle investigative work. Otherwise it’s too easy for a data scientist to go down a rabbit hole and spend a lot of time producing nothing.

Also, if your data scientist can’t run experiments quickly then they’ll struggle to fit their work within an agile process, so this is another reason to make experimentation easy.

If the outcome of a particular piece of investigative work is particularly important (e.g. if getting it right will move the needle significantly on a success metric), then it’s fair to be more generous with the time you allocate. But it’s rare for it to be impossible to divide work up into small chunks.

Your data scientist should have a rough strategy in mind for how they want to perform the investigation, and this strategy can be used to codify specific tasks. This strategy won’t be set in stone, but it will still provide a good starting point.

Sometimes the outcome of data science work won’t be a piece of software but a set of insights to be used by, say, a marketing team. This work will still involve writing code and can be scoped and prioritised like any other software project.

### Data-driven decisions are a lie

It’s common for companies to claim that they make rational decisions based on data but in my experience very few companies are truly data-driven. This shouldn’t be very surprising -- companies are comprised of ordinary people, and ordinary people aren’t rational.

Try not to be one of the irrational people. The list of possible ways in which you can be biased would be [far too lengthy](https://en.wikipedia.org/wiki/List_of_cognitive_biases) a detour for this article, but _confirmation bias_ is a huge problem in this area.

It’s cathartic for me to talk about my experience with this, so excuse me while I rant for a few paragraphs...

Occasionally I’ll be given a data task by an important stakeholder as well as a set of thoughts on where to look first, what might be most predictive and so on.

I’m happy to incorporate any domain knowledge when engineering features, but I don’t assume that a feature will be predictive just because someone with a fancy title thinks it’s important.

Obviously I’m just as susceptible to confirmation bias as anyone else, so I try to put my own preconceptions aside and let the data decide what the real story is. It’s not always easy to apply statistical methodologies rigorously but it’s very necessary if you don’t want to draw the wrong conclusions.

All good, right? Wrong!

The problems start as soon as I present my work to the main stakeholder; it quickly becomes apparent that they’re only really looking for data to confirm the biases they already hold. I’ve always pushed back against this with mixed results.

The best-case scenario is that the stakeholder will defer to the person who’s supposed to be the expert with data (not being arrogant or anything, but that’d be me). Unfortunately, it’s somewhat more common to get overridden and any evidence that disagrees with existing assumptions ends up ignored.

At this point I just take the money and run.

In conclusion, it’s only human to be biased -- but if you’re aware of your own irrationality, you’re already halfway to solving the problem.

Your data scientist won’t always be right but don’t override them unless you’re completely sure of your ground. If you’ve hired someone good, it’s far more likely that they’ve drawn the correct conclusion from your data than you.

Much like in science, try not to fall in love with your own hypotheses and instead **let the data inform your decisions**.
