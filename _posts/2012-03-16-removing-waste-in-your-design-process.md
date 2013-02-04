---
layout: post
title: "Removing waste in your design process"
category: 
tags: []
reading_time: 9 min.
---
{% include JB/setup %}

<p class="callout">
Sketching, wireframing, Photoshop and HTML/CSS each have their place in certain phases of the process. In this post I want to give you an idea of which method to employ and highlight the advantages and pitfalls of each.
</p>

When I work on a feature or flow, I actively question my thoughts & decisions: _how does this get the job done?_ – _does it make sense?_ - _will it be easy to code?_ etc. If/when I catch myself making little or no progress towards a solution, I've found that it's usually because of a lack of feedback. As designers, we all know the feeling of "going in circles" and I consider this a wasteful part of the process.

Iterative design is all about spending as little effort as possible -but no less– to make an informed decision and then ship the work, so that our feedback loop(s) may tell us where to go next. So what exactly constitutes "as little effort as possible", and how can we minimize waste in the design process?

## Sketching

A simple sketch is the natural place to begin exploring possible solutions. Most of us keep a pad and pen readily available at all times, and for good reason – this is by far the fastest way to visualize your thoughts. However, the low fidelity of the good ol' sketch can sometimes hinder your ability to see if the direction you're taking is worth pursuing.

> A little sketching is an exploration, a lot of sketching is a procrastination
> <cite><a href="http://37signals.com/svn/posts/2241-a-little-sketching-is-an-exploration-a-lot">Ryan Singer</a></cite>

Sketching should be for quick explorations of abstract concepts, isolated UI elements or for outlining high-level flows (how does one get from A to B, what screens are necessary, etc.)

The sketch is also as a great vehicle for bouncing ideas off of  co-worker(s). These discussions then serve as a litmus test of how well you've thought through the proposed solution, and especially if it's time to move on to a higher fidelity. You should stop sketching if a teammate expresses the need to see things in greater detail, in order to see the big picture.

Remember, your sketch is just that: a doodle. This is why being able to recognize when to sketch, and when to _stop_ sketching, is crucial.

_aside:_

I personally prefer big, cardboard-like paper and a chisel-tip pen (danish shop for cheapskates, Tiger, has some great pads at DKK 50,-). This keeps me from thinking about the finer details too soon – much like premature optimization in programming, both of which should be considered wasteful.

I've tried out lots of iPad apps as well and found [Penultimate](http://itunes.apple.com/us/app/penultimate/id354098826?mt=8) and [Draft](http://itunes.apple.com/us/app/draft/id375570329?mt=8) to be my favorites - the [Ten One Pogo stylus](http://tenonedesign.com/stylus.php) is awesome for drawing on an iPad, by the way.
This is of less importance, of course - what matters is knowing when to sketch, when to stop and where to go next.

## Wireframing

The wireframe is a two-headed beast: the low production cost lets you quickly visualize details a simple sketch cannot provide, especially when mocking up interactions and how a user flows through the application. But the quick and cheap affordances of wireframing also provide an invite for features to creep in through the backdoor.

The sheer breadth of readymade widgets, UI components <sup><a href="#footnote1">1</a></sup> and even entire frameworks <sup><a href="#footnote2">2</a></sup> for apps like [OmniGraffle][], makes it painless to drag in a button here and a few tabs there (most often by request from stakeholders) – and before you know it, the budget is blown implementing all these things.

[omnigraffle]: http://www.omnigroup.com/products/omnigraffle

Such a souped-up wireframe will ultimately take on spec-like characteristics; everything in the wireframe is expected to be implemented. More often than not, such conditions are a root cause of an agile process turned waterfall.

Still, apps like Omnigraffle or [Balsamiq Mockups](http://www.balsamiq.com/) have no match when you need an easy way to visualize dynamic/JavaScript-driven interaction, eg. modal boxes, filling out forms, etc. – sometimes it pays to hold back on coding and explore a bit more by wireframing. The cost of trying out another idea is usually much lower in a wireframe, compared to a full-blown prototype in code.

Similarly, you may find yourself wanting to elaborate on a sketch, and need greater detail prior to moving into code and/or visuals. This is often the case when starting work on entirely new products, or large features, with no foundation to build upon and/or concepts that have yet to be fully understood.

The challenge obviously lies in striking the balance. Wireframes can and will often end up in too high fidelity - time wasted on details that would've been better spent on a real prototype in code.

<ol class="footnotes">
	<li id="footnote1"><a href="http://graffletopia.com/">Graffletopia</a> has an amazing collection of stencils for Omnigraffle</li>
	<li id="footnote2">Yahoo! maintains a <a href="http://developer.yahoo.com/ypatterns/about/stencils/">library of design patterns</a> in a wide array of formats.</li>
</ol>

## Photoshop

Over time, Photoshop has (d)evolved into little more than a necessary evil to me – it's a slow, bloated piece of software and it was never [a good fit for web design][app].

[app]: http://v4.jasonsantamaria.com/articles/a-real-web-design-application/ "Jason Santa Maria articulated this better than I ever could back in 2010"

My biggest issue with Photoshop is, and has always been, the lack of template hierarchy, page states and how nearly everything must be duplicated in order to be re-used. This enforces a focus on form _before_ function, and leads to things like filler text for body copy, near-identical .psd's with different filenames, etc.

As much as I try to avoid Photoshop, I feel that the necessary 20% of my time spent using it accounts for 80% of the waste in my process. Sure, this can be alleviated to some extent by applying some [best practices][etiquette] like sensible layer names, grouping, etc. – but there's just no way around the fact that simple changes quickly turn into huge tasks in your average .psd and this has always frustrated me.

[etiquette]: http://photoshopetiquette.com/ "Colloquially known as The Photoshop Etiquette"

I really only use PS for two things these days: rendering graphics that isn't feasible to do in HTML/CSS, and for quickly altering the layout/dimensions of many screen elements at once.

My approach to mocking up a page is somewhat backwards – where others might do most, or all, of their work in PS, I much prefer to mark up & style as much as possible, grab a screenshot and then move into PS. This remains the easiest way to try out broad changes to the layout and general look & feel. Whenever you need to do excessive search/replacing in the code to try an idea, Photoshop is most likely an easier way to test it.

_(Seeing how CSS preprocessing is proliferating these days, such global code changes are becoming less of a hassle with the advent of code re-use in stylesheets. That might prove to be another nail in the coffin for PS as an app for web design – more on that in a future post.)_



## HTML/CSS

Time spent mocking up a full page in Photoshop or wireframes can rarely be justified these days. Considering how many screen sizes we need to design for, I think we owe it to our stakeholders - and ourselves - to explore solutions in the natural habitat of web design, as early as possible.

I'm a big fan of designing in the browser for a number of reasons. For one, my assumptions about the UI instantly become tangible in a browser: real code, real issues. How should the app respond to a click, a form submission, etc.? These things become much more obvious when you can actually interact with the system, and not just a static representation of it.

There are limits to this approach, of course. Designing in the browser can also be a wasteful part of the process. As a rule of thumb, you should have a rough sketch to work from when you start coding. Whether the sketch is on paper, a wireframe or a .psd is not important - visualizing the concept you're implementing is what matters.

When you start building your prototype, being sloppy is a Good Thing. Crank out the HTML you need as fast as possible, keep the CSS inline and mostly concerned with structure - dimensions and floats/positioning. Once you've got the basic elements laid out, you can start making decisions about how the page or component will fulfill its job and start honing in on a solution to the problem.

You want to keep the code & visuals in a state that allows rapid changes in the early phase of your prototype build. This is why inline styles make sense in the beginning; a component is self-contained, can easily be moved and most importantly – quickly discarded, without any need for removing references to it in other files. Javascript functionality is best avoided early on - you don't want to get sucked up in some weird programming problem (and you will) when you're just exploring solutions.

The goal is to expend as little effort as possible to gain the insights you need to inform your decisions. Once you can commit to a solution, you can start to clean up your beautiful mess - this should mostly be a matter of extracting CSS to separate files, and maybe reconsidering the HTML tags you've used. For example, you might have marked up an unordered list (`<ul>`) that turned out to have an implicit order, thus an ordered list (`<ol>`) is a better fit. This is called [code refactoring].

[code refactoring]: http://en.wikipedia.org/wiki/Code_refactoring

## So, which method is the right one?

The approach you take should be proportional to the amount of confidence in your solution and your understanding of the problem space. We've all tried spending too much time fiddling with a Photoshop canvas, when we should've been drawing lines on paper. Or reworked some code snippet a million times over, when we should've been using some simple dummies in a wireframe.

I hope this has provoked some thoughts about your own design process and which methods you employ at a given phase.

If you want to observe a master at work, who makes all of this seem easy, I highly suggest watching [Ryan Singer's two-part Play by Play videos from PeepCode][rjs]. That session was a large inspiration to this post.

[rjs]: http://peepcode.com/products/ryan-singer-ux

Share your thoughts in the comments, on twitter or anywhere else you feel like it.

**Related reading**  
[Responsive Design Warrants a Change in Workflow][gb] — Gary Bacon  
[The Post-PSD Era][bf] — Brad Frost

[gb]: http://garybacon.com/post/responsive-design-warrants-a-change-in-workflow/
[bf]: http://bradfrostweb.com/blog/post/the-post-psd-era/