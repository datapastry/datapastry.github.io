---
title: "How to successfully deliver a data science project"
author: Iskander Yusof
excerpt: "And keep your data scientist happy at the same time."
header:
  overlay_image: /assets/images/header-pastry-9.jpg
  overlay_filter: 0.7
---

_(Continued from Parts [1]({{ site.baseurl }}{% post_url 2019-08-07-get-the-most-value-from-your-data-scientist %}) and [2]({{ site.baseurl }}{% post_url 2019-08-08-what-your-data-scientist-should-be-doing %}), where I explained how to onboard your data scientist and what they should be doing from day to day in order to deliver maximum value.)_

## Minimum viable data science

For your first data science project, your data scientist should ideally work through the entire process from building a machine learning model through to live deployment as quickly as possible (think weeks rather than months).

Avoid the temptation to prematurely optimise any particular aspect of the process. The project as a whole should be viewed as an MVP, i.e. the smallest amount of data science work that will conceivably move the needle on your success metric.

**You don’t need perfection in order to show concrete results.**

Once your data scientist has completed their first MVP, the end-to-end framework for building, deploying and evaluating machine learning models will be in place. They can then build on this and iteratively improve their data science solution over time.

Ensuring your data scientist’s work gets into production ASAP also means they’ll get visibility across the organisation very early on.

You’ll find that other stakeholders suddenly take much more of an interest in your data scientist’s output once they’ve put something concrete out into the real world. Expect to receive a lot of feedback of both the positive and negative variety!

All this will provide further fuel for your data scientist to improve the quality of their work.

On the flip side, if your data scientist doesn’t quickly put their models into production, then it’ll be a long time -- if ever -- before you see any kind of value from them. It’s common to see data scientists in this position wasting time on various theoretical exercises that go nowhere (or watching YouTube videos). This is very demoralising!

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
*   If you have a data analyst, put them next to your data scientist. It might be a bit scary for an analyst to also work in the engineering team, but most engineers are only really dangerous if provoked.
*   Facilitate easy communication between your data scientist and the relevant business/product folks.
*   Hire a data scientist who can put on their business hat and convince nontechnical stakeholders of the value of their work.

Incidentally, this team structure doesn’t need to change much if you have multiple data scientists.

You might want to designate one data scientist as a team lead but often this doesn’t make sense, e.g. if each data scientist is highly experienced and has ownership of their own projects.
{% include post_promo.html %}
### Tools of the job

You’ve probably heard of the expression “a poor craftsman blames their tools”, but as far as data science is concerned these are _not_ good words to live by.

You should aim to get your data, infrastructure and code into a shape where your data scientist can run experiments quickly in short iterations. At a rough guess, I would say that issues with tooling can decrease your data scientist’s productivity by a factor of up to 5. 

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

Also, if your data scientist can’t run experiments quickly then they’ll struggle to fit their investigative work within an agile process, so this is another reason to make experimentation easy.

If the outcome of a particular piece of investigative work is particularly important (e.g. if getting it right will move the needle significantly on a success metric), then it’s fair to be more generous with the time you allocate. But it’s rare for it to be impossible to divide work up into small chunks.

Your data scientist should have a rough strategy in mind for how they want to perform the investigation, and this strategy can be used to codify specific tasks. This strategy won’t be set in stone, but it will still provide a good starting point.

Sometimes the outcome of data science work won’t be a piece of software but a set of insights to be used by, say, a marketing team. This work will still involve writing code and can be scoped and prioritised like any other software project.

### Data-driven decisions are a lie

It’s common for companies to claim that they make rational decisions based on data but in my experience very few companies are truly data-driven. This shouldn’t be very surprising. Companies are comprised of ordinary people, and ordinary people aren’t rational.

But try not to be *too* irrational when drawing conclusions from data projects. The list of possible ways in which you can be biased would be [far too lengthy](https://en.wikipedia.org/wiki/List_of_cognitive_biases) a detour for this article, but _confirmation bias_ is a huge problem in this area.

It’s cathartic for me to talk about my experience with this, so excuse me while I ruin the end of this article by ranting for a few paragraphs...

Occasionally I’ll be given a data task by an important stakeholder as well as a set of thoughts on where to look first, what might be most predictive and so on.

I’m happy to incorporate any domain knowledge when engineering features, but I don’t assume that a feature will be predictive just because someone with a fancy title thinks it’s important.

Obviously I’m just as susceptible to confirmation bias as anyone else, so I try to put my own preconceptions aside and let the data decide what the real story is. It’s not always easy to apply statistical methodologies rigorously but it’s very necessary if you don’t want to draw the wrong conclusions.

All good, right? Wrong!

The problems start as soon as I present my work to the main stakeholder; it quickly becomes apparent that they’re only really looking for data to confirm the biases they already hold. I’ve always pushed back against this with mixed results.

The best-case scenario is that the stakeholder will defer to the person who’s supposed to be the expert with data (not being arrogant or anything, but that’d be me). Unfortunately, it’s somewhat more common to get overridden and any evidence that disagrees with existing assumptions ends up ignored.

At this point I just take the money and run.

In summary, it’s only human to be biased -- but if you’re aware of your own irrationality, you’re already halfway to solving the problem.

Your data scientist won’t always be right but don’t override them based on authority alone. *If* you’ve hired someone good, it’s far more likely that they’ve drawn the correct conclusions from your data than you.

Much like in science, try not to fall in love with your own hypotheses and instead **let the data inform your decisions**.

_(That's it for this article series! Stay tuned for future DataPastry articles: we'll explain how to do data science on a budget and how to design your data infrastructure to deliver max value for min effort._

_Want to discuss your own specific data problems? Book a [free consultation]({{ site.consultation_url }}) with us -- we're here to help!)_
{% include post_footer.html %}
