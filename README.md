
# Intro to HTML5 Applications

## Advice

### HP

- keep it high level
- assume your audience knows nothing about HTML5

### PC

- tell a story: beginning, middle, end
- what problem were we trying to solve?
- what did we do?
- what was the result?

## Slides

### Slide 1: Title Card

Introduction to HTML5 Applications

### Slide 2: Personal Intro

Andrew Burgess, I've been at RBC for about a year and a half. Work on Logan (Algo Trading Platform) primarily, the UI, and HTML5 application.

### Slide 3: Title

HTML5 is the best UI choice for your next application.

### Slide 4: What's the Problem?

## Notes

### What is the problem we are trying to solve?

The problem is that UIs are now something that everyone deals with all day
long.  Gone are the days of only working with a limited number of UIs, only
during working hours. Now, we use dozens of UIs daily; for many of us, it's
from the moment we wake up to the moment we fall asleep. More importantly, our
users are using dozens of UIs daily. They know what good UI/UX looks like.

And they expect that.

For many of us, we have a captive user base. The client support teams that use
the Logan UI can't use a different application to run commands or view orders.
But getting and keeping users isn't the only reason to have good UI/UX.

NOTE: this isn't really the only problem ... 

Why else?

- easy of use
- reduced developer involvement 

### What is an HTML5 Application?

Web application is UI build with HTML/CSS/JavaScript, accessed in browser via a URL, or in another browser-based wrapper (Electron).

All web applictions have at minimum two parts, or sides, which are:

- **client-side**: run in the user's browser. Responsible for rendering the UI, displaying the data, making requests or sending commands to the server.

- **server-side**: runs on your server. Responsible for serving the client-side application to the browser (via HTTP), querying databases, or other APIs (depending on your architecture), performing authentication and authorization. Common Frameworks: ruby on rails, django, spring boot, express, ASP.NET.

Either side here can do the heavy lifting: time was, the client side was thin, basically just forms you filled and submitted; the server side would do the heavy lifting. Now, more common to have thin server, that is basically just a proxy to the database.

#### Single Page Applications

You've probably heard of Single Page Applications (SPAs). Previously, there was a one-to-one relationship between URLs and the page that was viewed. Moving between the pages caused the browser to send a request to the server, for a new page (HTML/CSS/JS). Often, this meant that many of the common elements of your pages (styling, navigation, etc.) were part of every request. 

A SPA changes that: instead, of the page being a dumb output that is simply rendered, the initial request includes all the neccessary views. Switching no longer means reloading the entire page: it means just rendering the right view, which you already have in the browser. You might need to request data, but that raw payload (JSON/CSV/XML/text) is much smaller.

Mention WebSockes, other HTTP-alts here. 

Mention React / Angular here.

Pros / Cons?

### Why HTML5?

#### Open

The Web is open. This means several things:

The **Technology** is open: HTML / CSS / JavaScript specifications are not developed by single company, behind closed doors. Open standard, you can contribute as well!

https://github.com/tc39/proposals

These technologies aren't owned by a single company: when doing Windows (winforms, WPF, silverlight) or Mac (Cocoa API) development. Don't have to worry about how long a company will support and extend.

The **Tools** are open. Desktop dev, locked into specific tools:

- Windows: Visual Studio (example: co-op use JetBrains Rider, have to update winform UI in code, no interface builder.)
- Mac: XCode

With the web, tons of options. Free options (Atom, VSCode, Brackets), Commerial options (IntellJ/WebStorm, Sublime Text).

The **Libraries** are open. Literally hundreds of free libraries (can be a down-side, since many are poorly supported). One of the biggest open source communities. Example: React (driven by Facebook, but anyone can contribute: https://github.com/facebook/react/issues) Even libraries with paid support, 

Not just dev tools, but many libraries / frameworks as well. Anyone can contribute. Can get 

The **Source** is open: As we'll see in a second here, you can disect any web application you come across, because there's no compilation.

The **

web is OPEN - people will contribute. 


many free librarys: not enterprise support, but easy to get your hands on.

Always have access to the source code: example: grid lib, want to restyle, need to request the change from vendor. Can't reach into code and override manually. The web is open.

#### Faster Iteration

Demo: how easy to change code: change letter-spacing, img src, and background-color, marquee on home page.

JSP: change code, compile Java, deploy/restart. Started to have templates, but that's moving towards web-style.

#### Cross-platform

know people who want to switch to macbook here at RBC, but they can't do without several applications that require Windows. Don't let your app get in the way of people. 

Cross platform: not just for windows (or limited set of windows versions). Mobile (check), Tablet (check), Mac (check) Chromebook (check).

if you want to target the largest possible amount of people, use the web.

GET STATS: mac user count, win user count, web user count.

#### Performance - REASON NOT TO

easier, because abstracted, but comes at a perf cost. farther from the hardware (browser is like a second layer of VM?)
tradeoff is that it's cross-platform, because historically, limited system access (file systems, DBs, webcam, OS features). 

### Did you know? NEW HTML APIs

Let's wrap up with some of the cool things you might not know you can do in a web application. 

- Geolocation API
- Device motion and orientation events provide access to the built-in accelerometer, gyroscope, and compass in mobile devices.
- Push Notifications (toasts?)
- Video/Audio playback
- Video/Audio/Image capture
- native contextMenu
- web workers / shared workers / etc...

Using a wrapper like Electron / OpenFin? More APIs that you can take advantage of.

NOT JUST A WEBSITE

### Buzzwords?

- HTML5
- CSS3
- JavaScript / CoffeeScript / TypeScript
- Web Sockets
- Web Workers
- React
- Angular
- Web Assembly

## Brainstorm

Use EMS UI as example.

- Why build an HTML5 application (vs. what?)?
	- JavaScript: most commonly used langauge in the world, according to https://insights.stackoverflow.com/survey/2018/#technology

- What are the pros and cons?
	- "it runs fast videos on the interwebs" - HL

- What languages / technologies are used? (libraries, frameworks, build tools, etc.)

- What's the process of building an HTML5 application?
	- transpiling

### Audience 
- Some have done legacy web dev (server-driven web apps).
- Some with no clue about web dev.

Languages:
- Java / .NET: very strict
- JS: not strict at all
- HTML / CSS: separation of content and style (vs winforms, where content and style are tightly-coupled)

Java Swing: slow (garbage collections?)

Available Paradigms: OOP, Functional, diff worlds, diff paradigms.

example: thread vs event loop

2020 Strategy: we look at web tech for UI. years ago, only function mattered, because people looked at UIs during the day, at work. After that, not much. Now: we look at UIs all day every day. Especially mobile. And some of these experiences are really good! (Apple design awards?) Users know that it can be better. Used to good design, typography, familiar gestures / interactions (pull down to refresh (twitter, then Apple Mail). we need to use the tech that's used outside (if we want to keep up?) so that people are used to what they see. Use what they are familiar with, make it intuitive. 

... Never use outlook at home ...

Accessibility, Responsive: UI concepts born out of the web.

What do you wish you had known before getting into JS? https://news.ycombinator.com/item?id=17466391

https://developer.mozilla.org/en-US/docs/Web/Demos_of_open_web_technologies

https://www.w3.org/wiki/Open_Web_Platform

https://en.wikipedia.org/wiki/Usage_share_of_operating_systems