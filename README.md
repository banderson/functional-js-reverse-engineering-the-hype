## Functional JS: Reverse-engineering the Hype

_Begin with the End in Mind_. We'll use this age-old advice to examine the hype behind functional patterns in javascript. In place of mathematical proofs, we'll look at the results we can achieve with the tools available now, and dive into the functional ideas that drive them. The end goal is clear: to see if the hype is justified, we must look at how these patterns affect different parts of our front-end stack:

* Functional Rendering: fn(component, appState) == UI
* Data Management: Understandable data flow
* Performance: First simple, then FAST...

We can do all of this today with the tools and syntax we know and love, and there will be no shortage of recommendations on what to use and where to start.

Note: I am not affiliated in any way with the projects and libraries featured here, I just think they are the best options and want to give credit where credit is due.


---


# Random Notes:

* I've been the React guy, but I truly think the the patterns that are being introduced now, are going to be here for a while
* So, whatever time you put into "leveling-up" in terms of functional-patterns  will not be wasted, or a fad to be replaced by something else in 6 months
* However, that doesn't mean it will be easy; We have decades of OO patterns and libraries to lean on, we are sometimes in a brave new world with how to structure apps
* But remember: your app is still your app; we need to be smart about the core pieces not being fleeting
* Analogy: think back to 2008, with backbone: it was a small, evented, DOM-based MVC framework. What else was available at the time?
* But you weren't necessarily better off by ignoring it and waiting for angular; help create that future; programmoing in that way will lead you down a path; However, I think if backbone were **created** today, it would be laughed/scoffed at. Not because it's bad, but because it's minimal, and still requires work we don't want to do anymore;
* I think that's the world we're living in with React right now: it's minimal,  but it's not to be ignored; the patterns and principles behind it, I truly believe, are the next web.
* I won't be React, what we end up with, but you'll never have regretted following the road it took you down
* Begin with the end in mind: start with things like dev tools shown by

## Ideas:
* How to manage the AJAX stack (do ALL parsing in "DAO's")
* Jafar Husain on Object.observe stalling...
* Elm: using mutable data [wouldn't allow hot loading](http://mostlyerlang.com/2014/03/24/032-elm-with-evan-czaplicki/)
* https://twitter.com/worrydream/status/621765890187612160?refsrc=email&s=11


**Quote from Linus:**
"I will, in fact, claim that the difference between a bad programmer and a good one is whether he considers his code or his data structures more important. Bad programmers worry about the code. Good programmers worry about data structures and their relationships."
https://en.wikiquote.org/wiki/Linus_Torvalds
https://lwn.net/Articles/193245/

Primitive obsession: avoiding creating strong types



**Functional Javascript: Reverse-engineering the Hype**

_Begin with the End in Mind_. We'll use this timeless adage to examine the hype behind functional programming patterns in javascript. In place of mathematical proofs, we'll look at the end results we can achieve with todays tools, and dive into the functional ideas that drive them in all parts of our front-end stack:

* Functional Rendering: fn(component, appState) == UI
* Data Management: Data flow for humans
* Performance: First simple, then Fast

So leave the math textbooks at home, and get ready for a fast-paced tour of the tools and techniques you can use to get started with functional Javascript apps today.


### THE BIG IDEA:!!!!!!!!!!!!!!!!!!!!!!

Start off with Djjikstra Quote and and talk about what it means to make programming easier...

All examples should lead up to the finale, which is that the functional patterns we leverage are useful not because some mathematician says so or because it's the latest cool thing, but it's useful because it helps us overcome our limitation of managing systems over time.

BAM.


**NOTES**:
* Rendering: Return to the declarative UI "glory days"
    * UI is a Pure function
    * Summary of React stuff from fluent
    * Not just React, anything in paradigm is suited
    * DEMO: [Cosmos / Component Playground](https://twitter.com/reacteurope/status/620927691592761344?refsrc=email&s=11) with 2 way bound state, because components become pure functions
* Data Flow: Make our programs easier to understand
    * If our UIs are declarative and simpler, how does that extend to our entire app (data flow)
    * DEMO: using time travel to help fix bugs
        * Serialize/Export entire app state and import to replay
        * Add RSI calculation and generate events that will break it
        * Figure out an annoying bug for something like hover that is really hard to troubleshoot in-browser and use action replay to repro and fix
    * ALSO: change from thinking in _objects_ to thinking in _procedures_ (i.e. pure data objects that are passed into service objects that transform and return new objects)
* Keep our programs FAST
    * DEMO: Highlight on re-render to show immutable effects?
    * Discussion on lazy evaluation
* Do all of this with the tools and syntax we know and love
    * Review of features and libraries to use today
    * How can we tell when things change?
        * Jafar Husain on Object.observe stalling...
* Bonus benefits:
    * It translates to other languages/platforms
    * It's the "new norm"
        * Mutable paradigms are being replaced

