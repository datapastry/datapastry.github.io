---
title: "What your data scientist *should* be doing"
author: Iskander Yusof
excerpt: "Besides eating your pastries that is."
header:
  overlay_image: /assets/images/header-pastry-7.jpg
  overlay_filter: 0.7
---
_(Continued from [Part 1]({{ site.baseurl }}{% post_url 2019-08-07-get-the-most-value-from-your-data-scientist %}) of this series, where I explained how to onboard your data scientist so they're in a position to deliver business value ASAP.)_
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

If your data scientist has access to a large amount of clean, well-documented historical data on whatever it is you want to predict, then their job will be _much_ easier and they’ll be able to get to the next stage in no time at all.

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

<figure>
	<a href="{{ site.baseurl }}/assets/images/churn-data.png"><img src="{{ site.baseurl }}/assets/images/churn-data-small.png" alt="Example features for predicting churn"></a>
	<figcaption>Features for each customer and whether or not they churned. In reality there'd be a lot more rows, a lot more columns and everyone would have a slightly different definition of "churn".</figcaption>
</figure>

This is what they will use to build a machine learning model to predict churn. Hopefully their model will be awesome. But it’s also possible that their model will be rubbish.
{% include post_promo.html %}
### The prediction stage

In the churn example, you should expect that your data scientist will build a model that gives you an idea of who is most likely to churn.

By testing the model predictions on data it has never seen before, your data scientist should also have an idea of how accurate the model is. This is called “offline evaluation” (as opposed to “online evaluation”, where the model is tested after it has gone live).

Most likely the model won’t be perfectly accurate with its predictions, so you’ll need to discuss with your data scientist how much accuracy you need for it to be useful.

For many use cases you can still get a lot of utility out of a predictive model that is only slightly better than random guessing. On the other end of the spectrum, there are some problems for which you’ll require a very high level of accuracy.

To decide which category your problem falls into, your data scientist will need to work backwards from your definition of “success” and determine how much accuracy the predictive model needs to achieve this. It might indeed turn out that you don’t need an extremely accurate model to achieve what you want.

(Don’t forget that you should have [defined a success metric]({{ site.baseurl }}{% post_url 2019-08-07-get-the-most-value-from-your-data-scientist %}#success-metrics) during onboarding!)

There are also dozens of metrics for assessing the accuracy of a machine learning model. It’s your data scientist’s responsibility to figure out which metric is most suitable for your problem.

Try to ensure they give you at least a cartoon explanation of whatever metric they decide on. Also, don’t forget that this metric will usually not be the same as the success metric you agreed on during onboarding, although the two metrics should be clearly correlated.

**This is super-important to understand**, so here’s an example.

You might have defined success as minimising the “percentage of customers who churn in the next month”. And your data scientist’s metric will be aimed at determining how good their machine learning model is at finding out _which_ customers will churn.

But simply identifying these customers isn’t the same as preventing them from churning. To achieve your goal of reducing churn, you’ll need to take an action based on this knowledge.

The outcome of the data science project will depend on both the accuracy of the machine learning model _and_ how successful you are at _acting_ on the model’s insights to encourage customers to stick with your subscription service.

Which leads us nicely to the next step…

### The action stage

Once you’re happy with the model then you’ll need to “productionise” it in some way.

To do this, you’ll need to think about who is the _consumer_ of your data scientist’s work.

Is the machine learning model meant to be a single component of a larger software system, in which case your data scientist will need to collaborate with your software engineers?

Or will your data scientist be creating marketing segments to be used in campaigns run by your lead generation function?

Model productionisation (or “deployment”) is a large topic in its own right but it doesn’t necessarily have to be complex, at least in the first iteration. You _might_ need a data engineer but it isn’t always essential.

If you’re just starting out with machine learning then we’d recommend hiring a data scientist who can at least do the basics of model deployment, especially in situations where the data science function isn’t yet mission-critical.

This is particularly true now that deployment in cloud environments like AWS or GCP is easier than ever. You can always hire a data engineer once your data scientist has proved the value of their work and they start hitting the limits of their deployment knowledge.

### Online evaluation

The outcome of the action stage will be a productionised model that is integrated into your business in some way.

Once your data scientist’s model has gone live, its effectiveness should primarily be judged by your business-focused success metric. And this usually _won’t_ be the offline data science-specific metric your data scientist came up with in the prediction stage.

I know, I repeat myself, but this really is very important.

The last thing you want is to be discussing improvements in the Kullback-Leibler divergence (what?) when you really need to be focused on a plain-English metric like “percentage of churners”.

(Incidentally it’s common to monitor all sorts of metrics for a deployed model, including data science-specific metrics, but the purpose of this monitoring is primarily to ensure everything is running as expected.)

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

So now you have a new requirement for the churn model. It doesn’t just need to identify customers who are likely to churn, but it also needs to find churn-tastic customers who can _also_ plausibly be convinced to stay.

Now your data scientist will have to actually earn that high salary you’re paying them!

_(In the [final part]({{ site.baseurl }}{% post_url 2019-08-09-how-to-successfully-deliver-a-data-science-project %}) of this series, I'll talk about how to ensure your data science project is delivered successfully._

_Want to discuss your own specific data problems? Book a [free consultation](https://calendly.com/isk-pastry/consult) with us -- we're here to help!)_
{% include post_footer.html %}
