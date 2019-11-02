---
title: "What should a data scientist know?"
author: Iskander Yusof
excerpt: "Something about everything and everything about something."
header:
  overlay_image: /assets/images/header-pastry-5.jpg
  overlay_filter: 0.6
---
_(Continued from [Part 1]({{ site.baseurl }}{% post_url 2019-10-31-how-to-hire-a-data-scientist %}) of this series, where I explained how to test data scientists so you don't accidentally hire a baboon.)_
## Skills and experience

Data scientists are the ultimate jacks of all trades.

You don’t need someone who’s an expert in everything but it’s important that they understand how all the pieces fit together. **This is not a good field for extreme specialists**.

We’d advise customising the skills you test based on the specific role for which you’re hiring. You probably don’t need a data scientist with a deep knowledge of convolutional neural networks if they’re mostly going to be working on credit scoring.

Still, there are more similarities than differences in data science roles. Below you can find the types of skills and experience we’ve found to be especially relevant.

This is not intended to be an exhaustive list, nor should you expect to find a data scientist who ticks all these boxes. Again, we’d recommend tailoring your questions based on what is genuinely important for your specific role.


*   **Machine Learning**
    *   Knowledge of supervised learning (regression, classification) and unsupervised learning (clustering, dimensionality reduction) techniques
        *   Linear Regression, Naive Bayes, Decision Trees, Logistic Regression, SVM, k-NN, k-means, Random Forests, Gradient Boosted Trees, PCA, Gaussian Mixture Models...
    *   Being able to explain in depth how at least one ML model works
    *   Exploratory data analysis: what’s their approach?
    *   Building a model: what’s their approach?
    *   Feature selection/extraction
    *   Training, test, validation sets
    *   Cross-validation and bootstrapping
    *   How to assess the accuracy of an ML model
    *   Online and offline evaluation of ML models
    *   Can they relate ML-specific metrics to business metrics?
    *   Curse of dimensionality
    *   Overfitting
    *   Handling missing data
    *   Handling lots of observations/features
    *   Handling outliers
    *   Handling data quality issues: what’s their approach?
    *   Handling big data (too big to fit in memory): what’s their approach?
    *   Data wrangling/munging: how happy are they to work with messy data and get it into a suitable shape for analytics work?
*   **Tools**
    *   Comfortable with data science libraries such as numpy, pandas, sklearn
    *   Experience with cloud environments like AWS or GCP
    *   Experience with ML as a service (e.g. SageMaker, H2O or Cloud ML)
    *   Experience with relational databases and SQL
    *   Experience with NoSQL data stores like Elasticsearch or Redis
*   **Statistics**
    *   Hypothesis testing, confidence intervals, probability distributions (Gaussian, binomial, Poisson...), transforming distributions, basic probability theory, basic Bayesian statistics, correlation
    *   Measures of central tendency (mean, median, mode...) and dispersion (standard deviation, interquartile range…)
    *   Understanding of possible sources of bias
    *   How to run an A/B test
*   **Algorithms & Data Structures**
    *   Basic algorithms and data structures (sorting, searching, arrays, linked lists, stacks, queues, trees etc)
    *   Algorithmic complexity
    *   Recursion
    *   Dynamic programming
    *   Basic computer architecture (understanding the memory hierarchy, roughly what CPUs do etc)
*   **Maths**
    *   Linear algebra, multivariable calculus, [optimisation](https://en.wikipedia.org/wiki/Mathematical_optimization)
*   **Software Engineering**
    *   Ability to write clean, idiomatic Python
    *   Knowledge of another programming language (ideally a widely-used language very different from Python, such as Java or Scala)
    *   Tests (from “small” unit tests through to “large” integration tests)
    *   Version control
    *   Continuous integration and deployment
    *   An understanding of how to write reasonably efficient code
    *   Model deployment: how to get a machine learning model into production
    *   How much do they know about the kinds of issues you can run into with a productionised ML model? (e.g. drift, model updates, management of multiple models, monitoring accuracy metrics)
*   **Soft Skills**
    *   Verbal and written communication skills: how good are they at communicating technical subjects to a lay audience? **Can they communicate the value of what they do?**
    *   How much emphasis do they place on the tools and techniques they use vs. the business value generated from their work?
    *   **Process and management:**
        *   Experience leading teams/projects
        *   Experience working in an agile development environment
        *   Communication/management style
        *   Experience working with different stakeholders when delivering a data science project
    *   **Team structure:**
        *   Have they ever worked in a cross-functional team or have they always worked in pure data science teams?
        *   What has their relationship been with other data scientists, data engineers, data analysts or software engineers?
        *   Do they normally work solo or in close collaboration with others?
*   **Other**
    *   Specific industry experience, e.g. fintech or retail
    *   Specific knowledge of sister fields like NLP or computer vision
    *   Specific knowledge of “advanced” ML and statistical techniques such as deep learning or Bayesian inference
{% include post_promo.html %}
## The whole enchilada

These are steps we’d suggest using when hiring a data scientist. You don’t have to stick to this precisely; the only parts we’d view as being essential are the work sample test and ensuing discussion. 



1. **CV review**

    This is normally pretty easy and shouldn’t take more than a few minutes per CV once you know what to look for. Check the CV against your list of job requirements (which should also be in your job description!).

    If most of the requirements are satisfied, then you can move on to the next stage. Remember that the goal is to filter out obviously-poor candidates, not to identify great candidates at the very first stage.

2. **Phone screen**

    You’ll probably want a further screen to filter out dud candidates before taking the time to send them a work sample test.

    The idea of the phone screen is simply to eliminate candidates who are obviously not up to scratch or won’t be a good fit for some other reason. It’s a timesaving measure for both you and the candidate.

    We’ve found that a mix of questions about experience, a few specific technical questions and a short discussion of the role works well.

3. **Work sample test (ideally take-home)**

    Hmm. I talked about this in the [previous article]({{ site.baseurl }}{% post_url 2019-10-31-how-to-hire-a-data-scientist %}).

    TL; DR version: put together a concise test that’s representative of the job itself. And let us know if you’d like an example of a test and scoring rubric to use as a template.

4. **Presentation and discussion of results**

    No data science task would be complete without a presentation! The goal here should be to test the candidate’s communication skills and dive deeply into any questions you might have about the candidate’s work.

    It also makes it hard for candidates to pay other people to do the test for them.

5. **Technical interview (in person)**

    You usually won’t be able to put everything you want into a work sample test -- at least, not if you want the test to be doable in under 10 years.

    For this reason, you might want to conduct a separate technical interview to examine the applicant’s knowledge of software testing, model deployment and other topics.


    We don’t consider this to be as reliable an indicator as the work sample test, but it can serve as a useful tiebreaker if you have two very similar candidates. It might also be possible to incorporate the technical interview into the discussion of their work sample task.


    For more senior candidates -- especially those that will be leading projects -- the in-person interview is also a good opportunity to see where their priorities lie. Do they optimise for generating business value or are they more interested in technical concerns?


    A good way to assess this is to talk to the candidate about their past projects: do they emphasise the tools and algorithms they used? Or do they focus on the impact of their work?

    Technical acumen doesn’t always go hand in hand with having good business sense.

6. **Culture fit**

    Most data scientists are lovely and personable like us, but you do get the occasional lunatic. So you might want to get an idea of how the candidate will gel with your other team members before making them an offer.

    But make sure you have a clear idea of exactly what it is you mean by "culture fit" (make it part of your rubric!).

    “Didn’t fit the company culture” might just mean that the existing culture is a homogeneous old boys’ club and you'd subconsciously like to keep it that way.


### Keep evolving

Over time, you should be looking to improve your hiring practices so that you do a better job of selecting good candidates.

Realistically you can’t treat this as a data science problem (!) as you won’t have enough data points, but after making a hire it’s worth keeping an eye on how closely their work output corresponds with what you determined from your scoring rubric.

Did you over/underestimate their ability in any particular area? If so, you’ll want to figure out why and update your testing accordingly. 

Unfortunately it’s a lot harder to learn from the people you _didn’t_ hire as you’ll have no way of knowing how they might have performed had you given them the job. (If you have an idea of how to solve this problem, let us know.)

## But I’m not a data scientist!

For some reason lots of non-technical people believe they have the ability to hire good technical candidates.

They’re fooling themselves, unfortunately. The _only_ time I’ve seen this work consistently is when a hiring manager pays over the odds for data scientists with great portfolios.

I’ve been through many non-technical hiring processes as well as technical interviews. With the non-technical interviews, I usually have a strong sense that I could just as easily get the job after reading a few blog articles and saying a few buzzwords.

It also sets off a red flag in my mind: if the company doesn’t have a serious hiring process, what kinds of jokers will I be working with? (The reverse is also true. A good hiring process gives me a lot of confidence in a company.)

So how can you identify a good data scientist if you yourself are not a data scientist?

**Short answer:** You can’t. Your best bet is to hire someone with a great portfolio, but as mentioned this will likely cost you a small fortune because everyone else will want that person as well. It doesn’t take a genius to figure out that someone who used to run data science at Netflix and Airbnb is likely to be a pretty good data scientist.

**Long answer:** You can’t. At least not entirely on your own. You really need to find a way to get assistance from data scientists that you know and trust. If you’re not in a position to do this, then your best bet is to get in touch with us and we’ll happily play the role of “trusted data scientists”.

-----

It’s been too long since the last shameless plug, so I’ll conclude with a couple of paragraphs of marketing fluff.

If you do find yourself needing to hire a good data scientist -- and it _is_ hard! -- then [book a free consultation]({{ site.consultation_url }}) and we’ll help you out.

We’ll give you advice on hiring strategy (maybe you [don’t need a data scientist at all]({{ site.baseurl }}{% post_url 2019-10-06-you-dont-need-a-data-scientist %})) and build a structured interview and testing process tailored to your specific needs.

And if that’s not enough, we’ll even supply you with pastries.

Last but not least, we’re putting together a free *Hire a Data Scientist* package containing a sample work sample test (ha), objective scoring rubric and example job description.

You can use the *Hire a Data Scientist* package as a template for your own data science hiring needs. Just [subscribe below](#newsletter_subscribe) for DataPastry updates and we'll send the package to you when it's ready.

_(Want to discuss your own specific data problems? Book a [free consultation]({{ site.consultation_url }}) with us -- we're here to help!)_
{% include post_footer.html %}