---
layout: post
title: "Thoughts on the process #3: Photoshop"
category: 
tags: [Process]
description: Photoshop is a battletested go-to for screen designs, but has its time come around? Indulge me as I rant on a stable of visual artists everywhere.
reading_time: 3 min.
---
{% include JB/setup %}

<p class="callout">
<strong>Minimizing waste in the design cycle</strong>

This is the third in a series of posts about being efficient when exploring solutions to a design. Sketching, wireframing, Photoshop and HTML/CSS each have their place in certain phases of the process. I want to give you an idea of which method to employ and highlight the advantages and pitfalls of each.
</p>

Over time, Photoshop has (d)evolved into little more than a necessary evil to me – it's a slow, bloated piece of software and it was never [a good fit for web design][app].

[app]: http://v4.jasonsantamaria.com/articles/a-real-web-design-application/ "Jason Santa Maria articulated this better than I ever could back in 2010"

I really only use PS for two things these days: rendering graphics that isn't feasible to do in HTML/CSS, and for quickly altering the layout/dimensions of screen elements. The latter is what I want to expand on in this post - I call this the _hack'n'slash method_ (hat tip [Sebastian][]).

[sebastian]: http://twitter.com/stockmarr "Sebastian Stockmarr was the first I heard using this phrase."

I usually take a (somewhat) backwards approach to mocking up screens – where others might do most, or all, of their work in PS, I much prefer to mark up & style as much as possible in the browser, grab a screenshot and then move into PS.

The browser will always render the most accurate representation of the UI, but Photoshop remains the easiest way to try out broad changes to many elements at once. Radical changes to the layout, adjustments of the overall color scheme and similar "global" tweaks, all require excessive search/replacing in the code, which is hard to justify when you're just exploring solutions.

This is particularly true when I work on incremental changes and explorations in existing pages. In this regard, Photoshop still shines – especially combined with some of the other approaches I mention in these posts about the process.

_(Seeing how CSS preprocessing is proliferating these days, such global code changes are becoming less of a hassle with the advent of code re-use in stylesheets. That might prove to be another nail in the coffin for PS as an app for web design – more on that in a future post.)_

My biggest issue with Photoshop is, and has always been, the lack of template hierarchy, page states and how nearly everything must be duplicated in order to be re-used. This enforces a focus on form _before_ function, and leads to things like filler text for body copy, near-identical .PSD's with different filenames, etc.

As much as I try to avoid Photoshop, I feel that the necessary ~20% of my time spent using it accounts for ~80% of the waste in my process. Sure, this can be alleviated to some extent by applying some [best practices][etiquette] like sensible layer names, grouping, etc. – but there's just no way around the fact that simple changes in eg. CSS, quickly turn into huge tasks in your average .PSD and this has always frustrated me.

[etiquette]: http://photoshopetiquette.com/ "Colloquially known as The Photoshop Etiquette"

I've contemplated switching to Fireworks a lot, mostly because of the template-based approach and how it lets you define single, canonical, versions of UI components. Teaching an old dog new tricks is hard however, and I've never made the time to really get acquainted with the workflow in Fireworks.

I guess I'm stuck with Photoshop for the time being, and though it has served me well throughout the years, I expect this part of my workflow to change in the near future.