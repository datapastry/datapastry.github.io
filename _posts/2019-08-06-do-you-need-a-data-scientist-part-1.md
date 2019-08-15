---
title: "Do you really need a data scientist? _(1/3)_"
author: Iskander Yusof
excerpt: "Confessions of a data scientist."
header:
  overlay_image: /assets/images/header-pastry.jpg
  overlay_filter: 0.6
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
---
I have a confession to make. I hardly ever do data science.

This might sound like a bizarre claim, seeing as almost every job I’ve ever had has the words “Data Scientist” somewhere in its title.

_(Aside: “What exactly do I mean by “data science work”?_

_Well, the term is somewhat ill-defined but I usually use it to mean “something to do with machine learning”. This might include a healthy dose of data cleaning and feature engineering work in addition to model building itself.)_

So what’s going on? Am I getting paid a lot of money to watch YouTube videos of kittens all day long? No, of course not! I only spend 60% of my day on YouTube and most of the videos I watch are about other animals.

But let’s be serious for a few seconds.

As a Principal/Lead/Generally Quite Awesome Data Scientist, I receive a lot of requests for help with data science. Typically the conversation goes something like this:

**Me:** “HELLO I’M ISKANDER HOW MAY I HELP YOU!!!”

**Hiring manager:** “Er, hello there. Can you turn your mike down a bit?”

**Me:** “Oh, sorry. How may I help you?”

**HM:** “No worries. So we need someone who knows a lot about machine learning, and your background and experience sound like they’d be a great fit.”

**Me:** “Thanks, that’s nice to hear. Can you tell me a bit about your company?”

**HM:** “So we sell dragon food online. We’ve been in business for three years now and have been growing rapidly. Currently we sell tens of thousands of items a day.”

**Me:** “Sounds promising, I’ve actually been thinking of buying a dragon myself and I can see how this would be a good business. What would you like me to help with?”

**HM:** “Well, we’ve got a lot of data on our customers but have never really had the time to look into any of it properly. What we’d like you to do is look into it deeply and tell us what you can find.”

**Me:** “Cool. Did you have any specific use cases in mind, or would you like me to help you define these as well?”

**HM:** “We do have a couple of things in mind...”

_At this point I listen closely. I know that the first thing the HM mentions is likely to also be the highest-priority item for them, and hence the reason for the call._

**HM (continues):** “The most profitable area of business for us isn’t actually dragon food -- it’s the dragon training service we provide our customers.

"As you know, dragons are very much _en vogue_ now, but they have the unfortunate tendency to eat their owners. So we help customers train their dragons and reduce the likelihood of their getting eaten to less than 5%.”

**Me:** “Ah, I understand. So you want me to help you upsell customers to the dragon training service.”

**HM:** “Exactly! I can see why they call you a genius.”

**Me:** “Stop, you’re killing me. Can we talk about a few specifics? It sounds like you want me to figure out which customers are likely to purchase your dragon training service.

"Based on this, you’d be able to run marketing campaigns to acquire more customers like this, or even personalise your website so that **_DRAGON TRAINING SERVICE!!!_** pops up at exactly the right time for the right customer (unintrusively, of course).”

**HM:** “Yes!”

**Me:** “Right, so a good way to start might be to look at your existing customers and seeing which ones have bought the dragon training service, and then we can build a predictive model from there.

"Can I ask how many customers typically purchase the service at the moment?”

**HM:** “That’s actually tricky to answer. You see, the sale doesn’t actually happen online. Because it’s quite an expensive service, we feel it’s better to have one of our dragon trainers make the sale in person.

"So the sale itself is entered into our CRM, but often there’s quite a large delay between the sale actually being made and it actually getting logged into our system. The CRM itself is a legacy homegrown system and nobody likes to use it.”

**Me:** “I see. But it sounds like you should at least have a rough idea of sales figures, even if they’re not exactly up-to-date?”

**HM:** “Sure, it’s usually somewhere between 5 and 30 sales a month, depending on what campaigns are running.”

**Me:** “OK. That’s quite a small number of sales, and I can tell you straight away that it might be tricky to train a useful machine learning model on such a small number of positives.

"Has anyone looked at the profiles of existing purchasers manually, just to get a general feel for what kinds of buyers you currently have? Perhaps just by talking to them if nothing else?”

**HM:** “No, as I said nobody has had time to look at the data closely. That’s why we need a data scientist to really look into this more deeply.”

**Me:** “Ah, OK. Well, perhaps there’s another way we can look at this. Presumably the website functions as a lead generator of sorts, and then you have a dragon trainer who takes the lead and tries to make the sale.”

**HM:** “That’s pretty much it, yes.”

**Me:** “Right, it’s not ideal but we could view this as optimising two separate pieces. One is to maximise the number of leads generated by the website, and the other is to maximise the probability of a lead converting into a sale.

"Do you know how many leads you’re currently generating from the website?”

**HM:** “Yes, it’s a few thousand per month.”

**Me:** “Really? That sounds like a very low conversion rate, so it sounds like you either have a problem with the quality of leads or the follow-up needs to be improved?”

**HM:** “That is true, but the number of leads is one of the top KPIs for the website, so we’re trying to keep it as high as possible.”

**Me:** “Wouldn’t it make more sense to have the eventual number of dragon training sales be the KPI? You have to be careful with simply optimising the number of leads as you might end up with a lot of badly-converting leads.”

**HM:** “The sales data is in the CRM so we can’t track it as easily.”

**Me:** “Hmm, so it sounds like the first step is to fix this KPI as we need to make sure we’re optimising for something sensible. You mentioned that you have a CRM and presumably you also track visitor behaviour online?”

**HM:** “Yes, we use Google Analytics.”

**Me:** “Right, so in order to help you understand your sales, a data analyst -- because this is what I feel you really need before you hire a data scientist -- will ideally have all the data about each customer in one place.

"This is surprisingly difficult to do as it involves tracking customers as they proceed from the online world to the offline, and often this can’t be done retroactively."

**HM:** "OK..."

**Me:** "So as a first step, you might want to consider migrating to a better CRM that allows you to easily report your sales numbers and will also help to facilitate this online-to-offline tracking.

"Migrations are always tricky and I’m usually hesitant to recommend them, but clearly it’s hurting your business if you’re not even able to do reporting from your CRM. You’ll have to weigh the cost versus benefit of this of course.”

**HM:** “Thanks a lot, this all makes sense. So if we do proceed with this plan, would you be able to help us with the migration?”

**Me:** “I’ve done a few of these things before, but I’d suggest hiring a specialist instead as it’s obviously important for you and you don’t want to pay for data science skills that you’re not really using.”

**HM:** “That’s fine, we really need a data scientist as there’s a lot of scope for AI here as well. I didn’t tell you about the other work that needs to be done, which involves consolidating all our data sources...”

**Me:** “Erm… all right then. I’ve always wanted to learn more about CRMs.”

In reality, of course, I’d turn down any task where I didn’t think I was able to do a good job.

But weirdly, I’ve ended up “qualified” in a whole range of areas that have absolutely nothing to do with data science. This is because I’ve found myself doing “anything and everything to do with data”, and it’s not always obvious what a specific role will entail until you actually get started.

If I had to describe my working life in four sentences, it would be “I solve problems via any means possible. Usually with data. And I'm not very good at counting.”

I’m pretty happy with this as it makes me an easy hire in most situations, but the fact of the matter remains: I’m a data scientist who doesn’t often do data science.

_(In Parts [2]({{ site.baseurl }}{% post_url 2019-08-06-do-you-need-a-data-scientist-part-2 %}) and [3]({{ site.baseurl }}{% post_url 2019-08-06-do-you-need-a-data-scientist-part-3 %}) of this series, I'll talk about what data scientists **really** spend their time on. I'll also say more about when you **should** and **shouldn't** hire a data scientist._

_Want to discuss your own specific data problems? Book a [free consultation](https://calendly.com/isk-pastry/consult) with us -- we're here to help!)_