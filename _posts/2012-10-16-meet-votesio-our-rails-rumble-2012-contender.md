---
layout: post
title: "Meet Votes.io, our Rails Rumble 2012 contender"
category: 
tags: [railsrumble]
reading_time: 5:12 min.
---
{% include JB/setup %}

<figure>
	<img src="/images/rails-rumble-votes-io.jpg" alt="Image of Votes.io logo and mobile view">
	<figcaption><a href="http://votes.io/">Votes.io</a> is instant feedback. Quick polls. Fast answers.</figcaption>
</figure>

So the Rails Rumble 2012 is a wrap, and I'm really proud of what we've built.

[Votes.io](http://votes.io) is instant feedback: create a poll, share the short link and watch the results tick in, beautifully rendered in real-time.

## Embracing constraints

Working within a 48-hour constraint enforced a focus in the team on getting things done. Most of the team members, including yours truly, have toddlers at home, further enhancing the time constraints and the focus on being über-productive.

Between diapers, family dinners and that pesky need for sleep, the task was simple: create a simple app that does one thing well.

## Removing friction.

We deliberately chose to not provide any account management or poll administration. Creating a poll should be dead simple — write a question, add some choices and share the link. Done.

Made a typo? Forgot to include a choice? No problem — just create a new poll. No messing around with deleting, editing or unpublishing a poll.

Sure, there's a lot of good reasons for tying votes to a user, and letting the creator go back and edit/update polls. It just wasn't right for this type of poll system. Votes.io was built for immediate responses to simple questions, and as such, each poll is shortlived.

The premises of the contest was also a factor in this decision. Judges can't be expected to invest a lot of time in each app, considering there's roughly 300 apps competing. I fear a lot of great apps in the Rumble will suffer a lack of votes, because of this.

## Designing the UI

<figure>
	<img src="/images/rails-rumble-usecases-votes-io.jpg" alt="Three different sketches of use cases for Votes.io">
	<figcaption>Use cases for Votes.io: Vote for tomorrow's lunch, get audience reactions and sending polls in emails.</figcaption>
</figure>

Our canonical use case is a speaker who creates a poll, prior to a presentation, and includes the URL in her slide deck. Then everyone vote simultaneously at the event and watch as results update instantly.

This focus on doing one thing well shines through in the UI, especially on the homepage. The interface is obvious and needs no further introduction:

<figure>
	<img src="/images/rails-rumble-votes-io-homepage.png" alt="">
	<figcaption>Votes.io homepage</figcaption>
</figure>

### Getting started

I initially hashed out some simple flows, to get a feel for the screens we'd need and what elements would be required to support the interactions:

<figure>
	<img src="/images/rails-rumble-userflows-votes-io.jpg" alt="Two diagrams of the user flows, needed to build the app">
	<figcaption>The flows needed for a minimally viable product</figcaption>
</figure>

After a couple of back-and-forths with the team, we started building the app. The rest of the team took on Rails and data modelling, and I started building the UI. For such a simple app, a quick sketch and then straight to code, felt like [the right approach](http://cabgfx.com/2012/03/16/removing-waste-in-your-design-process/).

<figure>
	<img src="/images/rails-rumble-campfire-sketches-votes-io.png" alt="A snapshot showing sketches posted to our chatroom">
	<figcaption>Quick sketch in Draft for iPad, post to Campfire for a quick discussion, then back to work. (In danish, sorry.)</figcaption>
</figure>

We didn't have time to design the UI from scratch, and decided to build off of Twitter Bootstrap. We'd get battle-tested components for free, eliminating potentially time-consuming issues. Bootstrap also provides a simple, pragmatic foundation for responsive design—a crucial factor for us.

<figure>
	<img src="/images/rails-rumble-copy-iterations-votes-io.jpg" alt="Four different snapshots of our iterations to body copy">
	<figcaption>Good copy is everything.</figcaption>
</figure>

### Feature freeze

At the end of Day One, we'd achieved our goal for the day: have a working, usable app. Still rough around the edges, but feature-complete. Create a poll; get a short link; watch results update in real-time, visualized in three different charts.

We started Day Two polishing the UI, refining copy, refactoring code and squashing bugs. We didn't quite manage to make all the visualizations really sing, so we decided to kill one of them. It's still in there, you might be able to find it ;)

As the end of Day Two was approaching, the app felt polished and we decided to ice the cake. We anticipated a lot of mistyped shortlinks (think thumbs vs. touch keyboards), so we added a little easter egg to our 404 page. We also added some featured polls to the frontpage.

### The cherry

With less than 3 hours left on the clock, I figured we could use a logo. I got busy with my Wacom stylus and [Paper for iPad](http://www.fiftythree.com/paper):

<figure>
	<img src="/images/rails-rumble-logo-iterations-votes-io.jpg" alt="Ideas for the logo and the final version">
	<figcaption>Combining bar charts to form the letter V</figcaption>
</figure>

And we had a logo. Admittedly, not the best logo I've made, but considering my caffeine level, it's alright. I used Jason Zimdars' [handy SCSS mixin](http://37signals.com/svn/posts/3271-easy-retina-ready-images-using-scss) to serve it @2x-dead simple.

We went trough the app, securing all pitfalls, tagged the repo and exhaled. Signed, sealed, delivered.

### Recommended.

This was my first time participating in the Rumble, and it's been great fun. I had a chance to try out some new techniques and just geek out for 48 hours. Bliss.

If you're a designer, you should definitely try joining a hackathon—it's not just for programmers. You might even pick up some new coding skills along the way, I sure did.

Huge props to the rest of Team Votes.io: Jacob Tjørnholm ([@chopmo][]), Laust Rud Jacobsen ([@laustrud][]) and especially Jakob Skjerning ([@mentalizer][]) for inviting me. Amazing what a simple retweet can lead to.

[@chopmo]: https://twitter.com/chopmo
[@laustrud]: https://twitter.com/laustrud
[@mentalizer]: https://twitter.com/mentalizer

Try out our app at [votes.io](http://votes.io) and if you think it's good, [please vote for us](http://railsrumble.com/entries/159-votes-io)—thanks!