---
layout: single-comment
title:  "ng-conf summary in words!"
author_profile: true
date:   2016-06-13 17:58:28 -0700
comments: true
---

Angular Conference: ng-Conf Salt Lake City May 4th-6th 2016

What is ng-conf?
Ng-conf is a 3 day Angular conference, created and hosted by people in the Angular community. Developers come from all over the world and Google’s core Angular team is leading the core talks and are there to give back to the community. It’s extremely well organized for having 1500 people attending and this year they had two full days of talks and one day with workshops you could pick and choose from. 

It's the best conference I've been to and hope to be back in the future!

I tried to keep the summary short and only include the most interesting things. This summary contains information gathered from talks, workshops, Q&As and hallway conversations. At the bottom, you’ll find links to videos if you want to do a deeper dive into any of the topics.

Executive Summary:

Angular 1 is a framework. Angular 2 is a platform!

Summary:

Angular 1 is a framework. Angular 2 is a platform!

Angular 2 is not just for the web, it can also be used for native mobile apps, hybrids mobile apps, progressive mobile apps and even desktop apps. It also supports server side rendering and you can switch the view layer for other options like React.

The size of Angular 2 is now ~45KB. That is smaller than ng1 thanks to the new offline compiler. Angular 2 is easier to learn and understand than Angular 1 (ng1). “Much of the tough stuff is not Angular.” Angular 1 had 43 directive and Angular 2 has two.

Angular 2 is fast. It renders 5 times faster than ng1 and change detection is now 10 times faster.

ngUpgrade makes it possible to have Angular 2 code in your Angular 1 application.

There is an Official Style Guide: https://angular.io/styleguide

Angular Universal will allow Angular to run on the server instead of the client. A server can render the page and just send over what should be displayed on the client without all the dependencies like libraries. The initial load and experience will be a lot faster. The client records all events while the real page loads and the events are played back to the actual page once it’s loaded. This is currently working with NodeJS and Asp.net, but will come to JBOSS/Wildfly soon as well.

Batarangle (the debugger for ng1) is rewritten for Angular 2 and called Augury (https://augury.angular.io/).

Angular 2 went from Beta to Release Candidate the day before the conference, you can follow the progress and future mile stones here: https://github.com/angular/angular/milestones

Angular CLI (https://cli.angular.io/) is a new command line interface for Angular 2. It will simplify how you build applications. To create a new application all you have to type is “ng new [appName]” and run it: “ng serve”. When you need to add components you use the “ng generate component” command.

Angular Mobile Toolkit allows you to create progressive mobile apps: Instant Loading, Offline capabilities, Installable and Notifications. Is this the future of mobile apps? Can this replace native apps?

Want to build Native apps? NativeScript was built on TypeScript and supports Angular 2. NativeScript converts Angular 2 code into the native iOS and Android API calls which are then executed as if you were writing a native mobile application in Objective-C (iOS) or Java (Android). If you don’t like NativeScript there are another options…. ReactNative!!!

If you prefer hybrids app over native apps, Ionic 2 is still a choice (http://ionic.io/2)

Electron allows you to package a JavaScript app for the desktop. This is cross platform solution that works on Windows, Mac and Linux. If you want see an example check out Visual Studio Code: https://code.visualstudio.com

The Angular Component Router was rewritten and the existing component router will be deprecated. The router doesn’t load your components till you need them. This means faster load of the application and you can now separate your concerns by adding the routing to individual components.

Material Design is used a lot on Android and an option to Bootstrap, but Angular Material for Angular 2 will not be ready till October.

Reactive Programming
Two-way databinding was a core concept of ng1. For those of you that played with early alpha version of Angular 2, you might have noticed that two-way databinding didn’t exist, it came later. Angular 2 fully supports functional/reactive patterns. If you like Redux you can use it, but there is now a stream based option for Angular called ngRx (https://github.com/ngrx).

AngularFire 2 is now in Beta (https://angularfire2.com/api/)
Is Firebase becoming the defacto standard as a backend prototyping database? (https://www.firebase.com/) Google Cloud is switching some of their services to Firebase.

If you going to learn Angular 2, you need to learn about Zones. Angular2 is built on it, it manages asynchronous tasks. It also allow for longer stack traces and ignores the $digest / $apply cycles and will also help with testing.

Codelyzer helps you finding problems in your code by checking your code against rules defined in your lint files. It’s now built into Angular CLI.

Angular 2 has a better way of supporting animations, see Matias talk below.

e2e Testing with Protractor. Protractor is an end-to-end test framework for AngularJS applications and works with Angular 2. Protractor is a Node.js program built on top of WebDriverJS (Selenium). Protractor runs tests against your application running in a real browser, interacting with it as a user would. Testing will be easier thanks to Zones. There is also plans add  headless mode to Chrome.

Is Angular 2 ready for production?
Google Fiber is using Angular 2, Google’s CRM app (Greentea) with over 100 developers is written in Angular 2 and now the AdWords team made the switch as well.



Here are links to the video of some of the more interesting talks

Key Note – Brad Green Jules Kremer
https://www.youtube.com/watch?v=gdlpE9vPQFs

Angular 2 – John Papa
https://www.youtube.com/watch?v=WAPQF_GA7Qg

TypeScript – Daniel Rosenwasser
https://www.youtube.com/watch?v=dzPjBWLdGz0

Angular 2 & Typescript – Dan Walin
https://www.youtube.com/watch?v=e3djIqAGqZo

Angular 2 – Scott Moss
https://www.youtube.com/watch?v=GE5gZX6V6Zs

New router – Misko Hevery
https://www.youtube.com/watch?v=d8yAdeshpcw

Augury Debugger
https://www.youtube.com/watch?v=b1YV9vJKXEA

Angular 1.5 components – Pater Bacon Darwin
https://www.youtube.com/watch?v=AMwjDibFxno

Testing – Julie Ralph
https://www.youtube.com/watch?v=DltUEDy7ItY

Angular Material – Kara Erickson
https://www.youtube.com/watch?v=rRiV_b3WsoY

Animations – Matias Niemela
https://www.youtube.com/watch?v=Hr4IKlr9mhg

React Native
https://www.youtube.com/watch?v=yDbaihb1eIs

Reactive Programming
https://www.youtube.com/watch?v=yEeDbHvg1vQ

Reactive Angular 2 (ngRx) – Rob Wormald
https://www.youtube.com/watch?v=mhA7zZ23Odw

Angular CLI
https://www.youtube.com/watch?v=wHZe6gGI5RY&list=PLvbhmfXjoKkdhhF_aHz8Ued1depHslamP

ng-Show - Shai Reznik
https://www.youtube.com/watch?v=aSFfLVxT5vA


All Slides & Code Samples

https://github.com/mikedice/ngconf2016-slides/blob/master/ngconf-slides.md


