---
title: Why bet on JavaScript vs. other languages in 2020?
published: false
description: Up to date advocacy on everyone's favourite ecosystem
tags:
//cover_image: https://direct_url_to_image.jpg
---

According to [dev.to](https://dev.to/t/javascript):

> Once relegated to the browser as one of the 3 core technologies of the web, JavaScript can now be found almost anywhere you find code.
>
> JavaScript developers move fast and push software development forward; they can be as opinionated as the frameworks they use

**As a software engineer in 2020, why should you invest or keep investing on JavaScript?**

-  **This post is not a troll**: it attempts to review JavaScript's unique strengths in depth with up-to-date infos

-  **Disclaimer**: 👨‍💻 I'm a fullstack web engineer so I'm obviously biased.

---

_**TL;DR:** In my opinion: The JavaScript ecosystem is better than ever and fulfils nearly every programming needs with ease and power. The associated trade-offs are very good. JavaScript is a valuable technology to invest on. JavaScript may be the best in the "all purpose" category at the moment, to the point that competing all-purpose languages are questioning their own relevance._

---

Now let's elaborate this advocacy, followed by a Q&A.

First, JavaScript is a **mere tool**. What we're after is:

1. the end goal: **solve problems through programming**
2. the side goal: **do it efficiently** = speed and ease of development, deployment, maintenance

JavaScript has a **unique** value proposition that all other programming ecosystem are trying to match but can't:

> With JavaScript, you can deliver **easy to use** solutions **to everyone**, **instantly** and of **high quality**.
>
> On the developer side, the language is **clean, logical, composes well**, is extremely **versatile**, has **unique strengths** and is **evolving healthily** with **increasing momentum**.
>
> The community is **huge** with **easy to consume** libraries for everything. The industry involvement is **also huge**. Last but not least: job opportunities are **huge** as well.
>
> Bonus: JavaScript is **lucky**.

Let's elaborate on those value points:

-  ⚡️ JavaScript apps are delivered **instantly**: as quick as typing a URL in a browser. **No installation needed**. Additional benefit: updates are seamless as well.

   -  In comparison: How would you would deliver your Python or Java solution to customers?
   -  Also: Web apps evades walled gardens such as the app stores.

-  👷🏻 JavaScript apps are accessible **to everyone**: every device has a pre-installed browser, everyone is familiar with accessing a web url and everyone has the permissions to do so. Even smartphones.

   -  In comparison: How would you get your mum to try your Java code?
   -  How would you get install rights for a corporate customer?

-  🧸 JavaScript apps are **easy to use** for the end user: I'm thinking about graphical UX here. JavaScript is integrated into browsers which are all about powerful and rich graphical user interfaces.

   -  In comparison: other languages painfully relies on clunky UI layers which pale in comparison of HTML/CSS.
   -  for additional end-user ease-of-use, JavaScripts apps can be packaged into mobile apps (PWA, Cordova, React native…) or desktop apps (Electron)

-  💎 JavaScript apps are **high quality**: look at facebook.com or atlassian.com, reliable, SpaceX

-  ✈️ The JavaScript language is **clean, logical and composes well**: TODO Kotlin borrowing the syntax

-  🤹‍♂️ The JavaScript ecosystem is extremely **versatile**

-  💪 The JavaScript language has **unique strengths** integrated async

-  🌱 The JavaScript language is **evolving healthily** ES5+ rejected

-  The JavaScript community is **huge**

-  industry involvement is **also huge**: AWS, facebook

-  JavaScript job opportunities are **huge**

## Trade offs

### But JavaScript needs a build step / some tooling

Unfortunately, due to its versatility, JavaScript usually needs some packaging before the final delivery, especially when targeting browsers. You may have heard of babel, webpack etc.

This is a very active area and the next progress stage for JavaScript.

When not targeting the browser (node) this is usually not a problem.

### constantly evolving

can be hard evaluating content found on the internet

### Too powerful / complexity of the ecosystem

The browser environment has a huge surface and one can't learn everything quickly. For a new starter, this can be daunting.

### dependency on npm

Not a problem so far.

### dependency on Google

Google controls nearly all JavaScript environments: Chrome (XX% shares) and node = Google v8

Google unilaterally adds and rejects APIs according to their needs and break the compatibility with competitors, cf. the browser wars.

If Google decides to promote a competitor to JavaScript (ex. Dart) they could easily harm JavaScript, for ex. reducing the SEO score of sites using it.

### The "JavaScript" name itself

Completely agree on that. That was a pitiful marketing attempt to borrow Java's fame at the time.

## Q&A

### But you're only talking about front-end

Not at all. Through node, JavaScript is a powerful backend solution thanks to its integrated reactor pattern that no other backend can match so far.

Also backend techs are driven by front-end techs + also tend to follow them, as Java did in the past, emerging as a front-end solution. Having the backend sharing the same language as its frontend is an obvious win, leading to the emergence of fullstack.

### But JavaScript is not as fast as _[some language]_

Execution speed is a common trade-off, nothing new here. JavaScript performs very well in its category of interpreted languages.

### But JavaScript has ugly parts such as === etc.

All languages have ugly parts https://wiki.theory.org/YourLanguageSucks

https://stackoverflow.com/questions/1995113/strangest-language-feature

TODO elaborate

### this drama story last month/year

TODO

### But JavaScript has no types

Types are just an aspect of a language. There are pros & cons as well.

TypeScript.

### Why not [some programming language]?

### Why not Python?

Pros:

1. top programming language of the moment according to some statistics
1. widely perceived as "easy to learn"
1. has some niche applications such as data processing or ML

Cons:

1. slower, no UI, no easy deployment
1. Python's niche are brittle, more luck than affinity

See [Python now needs to change](https://developers.slashdot.org/story/20/10/25/0239229/does-python-need-to-change):

> Python is the top language according to IEEE Spectrum's electrical engineering audience, yet you can't run Python in a browser and you can't easily run it on a smartphone. Plus no one builds games in Python these days (…)
>
> Despite Python's success as a language (...) it's at risk of losing its appeal as a general-purpose programming language and being relegated to a specific domain, such as Wolfram's Mathematica, which has also found a niche in data science and machine learning...
>
> (...) "It's an embarrassing admission, but it's incredibly awkward to use Python to build and distribute any applications that have actual graphical user interfaces," he tells ZDNet. "On desktops, Python is never the first-class language of the operating system, and it must resort to third-party frameworks (…)" Packaging and redistribution of Python desktop applications are also really difficult (...)

### Why not Java?

Pros:

1. Java is slightly faster, can handle bigger workloads and is more established/stable

Cons:

1. Java starts to feel its age: old syntax, old paradigms (OOP), no easy async
1. Java is not integrated in browsers, it needs an install steps and corresponding permissions
1. Java is now suffering what it once did to previous language: leveraging front-end dominance to win the back-end

> Aging programming languages suffer from a bad plastic surgery addiction. They are desperately injecting new features in the fevered hope of remaining popular, or at least fashionable. (…) I think that we should instead praise JavaScript’s inner beauty.

For example, see Java painful attempt to add lambda syntax while maintaining backward compatibility: TODO link

Also see [The war for the browser, Oct. 2020](https://developers.slashdot.org/story/20/10/25/190257/java-geeks-discuss-the-war-for-the-browser-and-the-state-of-java-modularization)

> Java is in a war for the browser. Can it regain the place it once held in its heyday?
>
> All major browsers have disabled support for Java (and indeed most non-JavaScript technologies). Web-based front-ends are usually coded in JavaScript (…) Yes, (…) you can generate [websites] using Java libraries and business logic, but once it is sent to the browser it is static and lifeless... Java client-side innovation has all but stopped, at least via the official channels....
>
> How can Java increase its relevance? How can Java win back client-side developers? How can Java prevent other technologies from leveraging front-end dominance to win the back-end, like Java once did to other technologies?
>
> To win the war, Java needs a strong client-side option. One that lets developers make modern web applications using Java code. One that leverages web technologies. One that supports components. One that builds quickly. One that produces fast-downloading, high performance, 100-Lighthouse-scoring apps. One that plays nicely with other JVM languages...

### Why not C++

Pros:

1. speed, C++ is a compiled language in a completely different category

Cons:

1. all the usual:
1. C++ is aging and hard to evolve

### Why not Golang?

### JavaScript is not a serious language
