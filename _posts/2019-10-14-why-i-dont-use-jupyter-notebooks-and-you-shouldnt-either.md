---
title: "Why I don't use Jupyter notebooks and you shouldn't either"
author: Daoud Clarke
excerpt: "Jupyter notebooks give you instant feedback but lead to bad habits."
header:
  overlay_image: /assets/images/header-article.jpg
  overlay_filter: 0.6
---

Why I don't use Jupyter notebooks and you shouldn't either
==========================================================

Jupyter notebooks are pretty much the first tool a data scientist
pulls off the shelf when approaching a new problem. And with good
reason. There's nothing like the immediate feedback you get when you
press shift-enter and your code is evaluated. Plus, you can see your
graphs right there next to your code! What's not to love?

Well, quite a lot.

I'm a data scientist, but I very rarely use Jupyter notebooks. Here's
why, and why I think you shouldn't use them either if you want to be
the most effective data scientist you can be.


They encourage polluting the global namespace
---------------------------------------------

The best feature of notebooks is that they provide instant feedback:
just press shift-enter.

This is also their worst feature.

In order to get that instant feedback, I find myself writing code in
the global namespace, instead of writing functions. This is generally
[considered bad practice](https://stackoverflow.com/a/19158418) in
python development. The reason for that is that it's very hard to
reason about the effect of running a sequence of cells. They're all
modifying the global namespace, which means your notebook is
effectively a horribly large [state
machine](https://en.wikipedia.org/wiki/Finite-state_machine).

It also leads to my next two objections...


They discourage effective code reuse
------------------------------------

The best way to reuse code in python is through functions and
classes. In notebooks, the temptation is to reuse code through _cells_
instead. Because you're using the global namespace, you are relying on
cells being executed in a particular order. In order to reuse code in
cells, you would have to set some global variable then run the right
cell. Keeping track of what needs to be run and in what order then
becomes a problem, and also leads to...


They harm reproducibility
-------------------------

If you always run your notebook in a linear order from start to finish
then reproducibility shouldn't be an issue. Someone else can take your
notebook, run it in order, and get the same results.

However (see above) this means that you typically won't have great
code reuse. It also somewhat defeats one of the benefits of using a
notebook, which is that you can run it in whatever order you like.

If you don't always run it linearly then someone else running your
notebook may well run it in a different order too, and it's hard to
make sure they will then get the same (or at least valid) results.

You care about reproducibility right? You're a data _scientist_.


They don't play nicely with source control
------------------------------------------

If you're a professional data scientist you probably work in a
team. That means you need to collaborate. And collaborating with
notebooks is... rubbish. Generally it means saving the notebook and
sending it to someone.

Of course you can put notebooks into source control. As long as no-one
else is editing it at the same time, in which case, good luck trying
to merge with their changes.


They're not PyCharm
-------------------

So if you shouldn't use notebooks, what _should_ you use?

I haven't found anything better than PyCharm. It effortlessly
translates my thoughts into code. Ok, maybe it's not quite that easy,
but it does have some amazing features that are sorely missed whenever
I'm forced to use a notebook:

 - Proper code completion (not the rubbish you get when you press tab
   in a notebook).
 - Automatic renaming of variables
 - Search the entire codebase for a function or class
 - Refactor to extract a method or function

...amongst many other things.

But what about the joy of pressing shift-enter? I need my dopamine hit!

If you really need the interactive-ness notebooks, you can pay for the
professional edition, which has a "scientific mode". This includes the
ability to view matplotlib graphs and pandas dataframes. You can even
run notebooks from within PyCharm if you really want to.

But you don't want to, do you?

_(Want to discuss your own specific data problems? Book a [free consultation]({{ site.consultation_url }}) with us -- we're here to help!)_
{% include post_footer.html %}
