---
layout: post
title: "Thoughts on the process #2: Wireframing"
category: 
tags: [Process]
reading_time: 3 min.
description: Wireframes are great for lots of things in the design process – but they tend to create a false sense of agreement when employed in the wrong settings.
---
{% include JB/setup %}

<p class="callout">
<strong>Minimizing waste in the design cycle</strong>

This is the second in a series of posts about being efficient when exploring solutions to a design. Sketching, wireframing, Photoshop and HTML/CSS each have their place in certain phases of the process. I want to give you an idea of which method to employ and highlight the advantages and pitfalls of each.
</p>

The wireframe is a two-headed beast: the low production cost lets you quickly visualize details a simple sketch cannot provide, especially when mocking up interactions and how a user flows through the application. But the quick and cheap affordances of wireframing also provide an invite for features to creep in through the backdoor.

The sheer breadth of readymade widgets, UI components <sup><a href="#footnote1">1</a></sup> and even entire frameworks <sup><a href="#footnote2">2</a></sup> for apps like [OmniGraffle][], makes it painless to drag in a button here and a few tabs there (most often by request from stakeholders) – and before you know it, the budget is blown implementing all these things.

[omnigraffle]: http://www.omnigroup.com/products/omnigraffle

Such a souped-up wireframe enables mutual agreement in a meeting, but will ultimately take on spec-like characteristics; everything in the wireframe is expected to be implemented. More often than not, I've found such conditions to be a root cause of iterative development turned waterfall.

The challenge obviously lies in striking the balance. I've found that my wireframes often end up in too high fidelity - time wasted on details that would've been better spent on a real prototype in code.

Still, apps like Omnigraffle or [Balsamiq Mockups][] have no match when you aren't ready to start coding, but still need an easy way to visualize dynamic/JavaScript-driven interaction, eg. modal boxes, filling out forms, etc.

[balsamiq mockups]: http://www.balsamiq.com/

Similarly, you may find yourself wanting to elaborate on a sketch, and need greater detail prior to moving into code and/or visuals. This is often the case when starting work on entirely new products, or large features, with no foundation to build upon and/or concepts that have yet to be fully understood. 

If you're a hybrid designer/developer like me, backend- and frontend-development is done more or less in parallel, and sometimes it pays to hold back on the coding and explore a bit more by wireframing.

When you're exploring a solution, your first pass might fail to capture an accurate model of your domain. In these situations the cost of trying another direction is usually much lower in a wireframe, compared to a full-blown prototype in code.

Due to my prior experiences with wireframes I tend to avoid them these days, going straight to markup for all my prototyping. But lately I've somehow felt they'd have been a better fit on a couple of recent projects.

I'll probably resurrect my copy of Omnigraffle very soon, as I'm about to take on the daunting task of redesigning the 6-step(!) registration flow on [Autobutler.dk](http://www.autobutler.dk). I hope to follow up this post with my experiences.

<ol class="footnotes">
	<li id="footnote1"><a href="http://graffletopia.com/">Graffletopia</a> has an amazing collection of stencils for Omnigraffle</li>
	<li id="footnote2">Yahoo! maintains a <a href="http://developer.yahoo.com/ypatterns/about/stencils/">library of design patterns</a> in a wide array of formats.</li>
</ol>