---
layout: post
title: "A review of the new Basecamp"
category: 
tags: [apps, review]
reading_time: 7:30 min.
---
{% include JB/setup %}

**TL;DR** The new Basecamp from 37signals is out, and I've been using it for about a month now. It's an amazing product and, pending some minor tweaks & additions, poised to become the new standard for project management tools to adhere to.

> Most project are small and short. The original Basecamp was overkill for most kinds of projects. The new Basecamp is perfect for projects of every size.
> <cite><a href="http://37signals.com/svn/posts/3129-launch-the-all-new-basecamp">Jason Fried</a>, in the launch post on Signals vs. Noise (company blog).</cite>

I've used the original Basecamp (now renamed to Basecamp Classic) for a long time and I always had mixed feelings about it. It did a lot of things well, but as a whole, it often felt like a drag; keeping Basecamp updated became a task of its own.

Boy, has that changed.

## Rewrite
The team at 37signals decided to start from scratch with the new Basecamp (initially dubbed Basecamp Next, or BCX, for short), and launched it as a separate product from the Classic edition, which is still available and maintained. That is a bold move: it takes balls to decide to rewrite your flagship offering, one that's been profitable for 8 years and counting. Gotta respect that.

It's interesting to see a company with the clout of 37signals take on The Big Rewrite, and they've done a very good job. Chris Bliss of VM Associates [wrote a great post][vm] about their execution, which he thinks is (sort of) revolutionary:

[vm]: http://www.vm-associates.com/2012/03/15/basecamp-software-cloud-consulting-37signals/

> Once the product felt dated (after ~8 years, or roughly 3 cycles in the old model) they built a brand new product from the ground up. They combined the best of both worlds: the quick feedback loop of the new model with the “ground up” approach of the old model. Brilliant.

## Focus & Simplicity
The number one reason I love BCX is how it exudes simplicity and feels powerful at the same time. Every feature clearly had to fight to make the cut, which leaves a razor-sharp focus on getting things done.

A lot of people are up in arms about features from Classic that's not in BCX, such as private items, time-tracking and Milestones (to-dos tied to an event) – all features I rarely used myself, and the app seems better off without them. It feels like a lean and focused app that complements, rather than compromise, my workflow – checking in to catch up or post an update is now quick and effortless, which was rarely the case in the past.

## Snappy UI

Part of this is because of the speed and responsiveness of the interface – Basecamp is stupid fast, due to some solid engineering with sophisticated [HTML5 pushState wizardry][push] on top of [a ridiculous amount of RAM][ram] used in [an interesting approach to caching][caching]. Did I mention how fast it is?

[push]: http://37signals.com/svn/posts/3112-how-basecamp-next-got-to-be-so-damn-fast-without-using-much-client-side-ui
[ram]: http://37signals.com/svn/posts/3090-basecamp-nexts-caching-hardware
[caching]: http://37signals.com/svn/posts/3113-how-key-based-cache-expiration-works

Attractive things work better, and the new Basecamp is testament to that. The interface is gorgeous and a joy to use, mainly because of how unobtrusive it is. Generous use of whitespace and excellent choice in colors & typography combine to form a layout that's pleasant to work with and most importantly–gets out of my way.

There's a lot of great details in the UI, but one that stands out is what 37signals calls _page-stacking_ - pages as sheets of paper. This is a truly innovative approach, and it works really well. [This video][vid] explains it way better than I ever could (jump to 3:20).

[vid]: http://www.vimeo.com/36917486

## Human-friendly

Too many people are slaves to their email, but I totally get why most people stick with it; it's easy and it Just Works (most of the time). I've tried suggesting tools like Basecamp to these people, with the same outcome every time: busy people can't be bothered to take a new system in until the benefits are proven.

Now, people don't have to adapt to a new system at all if it doesn't work for them. Basecamp works incredibly well as a transparent layer on top of the regular flow of emails - I've been using it with my team at autobutler.dk since launch, and we've had none of the pushback from the last time we tried to introduce Basecamp (when only Classic was available). Some team members use Basecamp, others just use Gmail, and all of our progress on projects is recorded and gathered nicely in BCX.

This is in large part due to a new feature called **Loop-in**.
Here's how it works: you post something in BCX, and want to let others know about it. You tick off the usual suspects to be notified, and in addition to that, you can notify (loop-in) someone that's not on the project by adding their email to the list of recipients:

<figure>
	<img src="/images/new-basecamp-loop-in-feature.png" alt="Image of how Basecamp's new loop-in feature works">
	<figcaption>The new loop-in feature in Basecamp</figcaption>
</figure>

They'll get an email with the entire conversation in reverse chronological order, and can just reply to that email. Business as usual. This works really well, even more so for when you want to include someone that's not even a part of your company.

## Overview

Another great feature is the _Daily Progress_ page, accessible from the main navigation. This is the successor to the Dashboard in BCC, and is way better - it was called _Timeline_ during the beta, which describes what type of overview it provides.

This global overview is complimented by each project's _Catch up on recent changes_ page, that lists activity day-by-day. Additionally, almost all actions in Basecamp are covered by an audit trail and undoable history, so you quickly become confident that data won't ever wind up missing, once it's been put in Basecamp.

Another thing that works well is how Discussions are aggregated on the main project page from all comments, on all items. This is especially great compared to the old Dashboard and Messages index, both tedious to go through when you just needed to get an idea of what was currently being discussed.

You can also have a daily catch-up mail sent to you at 7am with yesterdays progress and as always, you subscribe to RSS feeds of your projects activity. All of these things might seem a bit daunting at first, but they're not. Apart from the occasional overflow of emails, the team at 37signals seems to have struck a near-perfect balance with regards to how and when you catch up on a project.

## Quirks

As I mentioned in the start of this post, there are some parts of the new Basecamp that rub me the wrong way. But the fact that they're all minor details, speaks volumes about the quality of the first release.

First of all, the administration of people and their permissions/project access is a bit wonky. For example, new invitees are granted permission to create new projects by default - that surprised me a bit, but it's not that bad. However, when compared with the fact that new projects aren't visible to me, an Administrator _and_ the account owner, it becomes weird. Regardless of your role & permissions in the account, you can only see projects to which you've been granted access. That just doesn't feel right, especially on accounts with a set project limit.

Generally speaking, I sometimes get lost navigating between sheets (pages). I tried narrowing it down to a specific example/scenario, but I couldn't – it's just one of those things that's hard to explain until you try it yourself.

I might be biased from using the Classic version, but I initially thought Todo-lists weren't sortable by dragging and dropping - there's no visual clues that you can do this on the items in the list. This goes for the entire list as well - they both afford clicking much more than dragging.

It also really bugs me that there's no apparent way to delete files - it's not a problem right now, but it will be once I've used a sufficient amount of the storage in my account.

Finally, I miss some mobile optimizations - but given that this is version 1.0, and that the new API was recently released, I'm confident that we'll see some efforts in this area soon.


## 9/10

Overall, it's been a long time since I was this impressed with the initial release of an app - the high expectations I had, have definitely been met.

I had the pleasure of participating in the closed beta, and it's been really fascinating to get an inside peek of how 37signals prioritize their efforts and push back on feature creep. Their approach to building a great user experience leaves no room for compromise and it shows in the product.

If you haven't used Basecamp before, or if you're still using the Classic version, now is the time to switch. With a 45-day trial and a price starting at $20, it's a no-brainer.