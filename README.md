
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

All web applictions have at minimum two parts, or sides, which are:

- **client-side**: run in the user's browser. Responsible for rendering the UI, displaying the data, making requests or sending commands to the server.

- **server-side**: runs on your server. Responsible for serving the client-side application to the browser (via HTTP), querying databases, or other APIs (depending on your architecture), performing authentication and authorization. 

Either side here can do the heavy lifting: time was, the client side was thin, basically just forms you filled and submitted; the server side would do the heavy lifting. Now, more common to have thin server, that is basically just a proxy to the database.

#### Single Page Applications

You've probably heard of Single Page Applications (SPAs). Previously, there was a one-to-one relationship between URLs and the page that was viewed. Moving between the pages caused the browser to send a request to the server, for a new page (HTML/CSS/JS). Often, this meant that many of the common elements of your pages (styling, navigation, etc.) were part of every request. 

A SPA changes that: instead, of the page being a dumb output that is simply rendered, the initial request includes all the neccessary views. Switching no longer means reloading the entire page: it means just rendering the right view, which you already have in the browser. You might need to request data, but that raw payload (JSON/CSV/XML/text) is much smaller.

Pros / Cons?


### How does it solve the problem?



### Did you know?

Let's wrap up with some of the cool things you might not know you can do in a web application. 

- Geolocation API
- Device motion and orientation events provide access to the built-in accelerometer, gyroscope, and compass in mobile devices.
- Push Notifications (toasts?)
- Video/Audio playback
- Video/Audio/Image capture
- native contextMenu
- web workers / shared workers / etc...



## Brainstorm

Main Message: HTML5 is the best UI choice for your next application

- What is HTML5 / an HTML5 application?
	- graphical User Interface accessed via the browser (or another web wrapper)
	- often described as a front-end vs. back-end, which are two seperate apps that are often tightly coupled.
	- front-end: UI build on web technologies: HTML, CSS, JavaScript
	- back-end: any web server (ruby on rails, django, spring boot, express, ASP.NET?)

- Why build an HTML5 application (vs. what?)?
	- JavaScript: most commonly used langauge in the world, according to https://insights.stackoverflow.com/survey/2018/#technology
	- 

- How is it different from a traditional GUI?
	- Deployment: deployed to a server, accessed via a browser.
	- 


- What are the pros and cons?
	- "it runs fast videos on the interwebs" - HL

- What languages / technologies are used? (libraries, frameworks, build tools, etc.)
	- 

- What's the process of building an HTML5 application?
	- transpiling
	- 

- How does this relate to ...?
	- 


- Briefly demo Logan's architecture
- Common Technologies / Buzzwords
	 - HTML5
	 - CSS(3)
	 - JavaScript / TypeScript
	 - Web Sockets
	 - React / Angular
	 - 

# Audience 
- Some have done legacy web dev (server-driven web apps).
- Some with no clue about web dev.

Single Page Application (SPA) - what is that, how into tools they have heard about (React / Angular)

Why web over desktop? take .NET (winforms, WPF, silverlight) - all owned by a single company, how long will they support these technologies? continue to provide new features?

web is OPEN - people will contribute. 

desktop is CLOSED - vendor lock-in, tools lock in (Visual Studio). (ex: co-op is using ryder, have to update winForms UI by hand, in code)

Iteration: can tweak a web app in Chrome, change HTML / CSS, interact with UI fast. better, more diverse tooling

Cross platform: not just for windows (or limited set of windows versions). Mobile (check), Tablet (check), Mac (check) Chromebook (check).

many free librarys: not enterprise support, but easy to get your hands on.

if you want to target the largest possible amount of people, use the web. stats: mac user count, win user count, web user count.

Demo: how easy to change code.

JSP: change code, compile Java, deploy/restart. Started to have templates, but that's moving towards web-style.

Languages:
- Java / .NET: very strict
- JS: not strict at all
- HTML / CSS: separation of content and style (vs winforms, where content and style are tightly-coupled)

Only One Problem ... Performance

easier, because abstracted, but comes at a perf cost. farther from the hardware (browser is like a second layer of VM?)
tradeoff is that it's cross-platform, because historically, limited system access (file systems, DBs, webcam, OS features). 

However, more recently, as part of HTML5, more new APIs. Did you know ... (not just a website)

OpenFin, Electron: more APIs, b/c "desktop" wrappers.

Web Assembly?

(don't mention tooling, muddies the waters)

Java Swing: slow (garbage collections?)

Available Paradigms: OOP, Functional, diff worlds, diff paradigms.

example: thread vs event loop

2020 Strategy: we look at web tech for UI. years ago, only function mattered, because people looked at UIs during the day, at work. After that, not much. Now: we look at UIs all day every day. Especially mobile. And some of these experiences are really good! (Apple design awards?) Users know that it can be better. Used to good design, typography, familiar gestures / interactions (pull down to refresh (twitter, then Apple Mail). we need to use the tech that's used outside (if we want to keep up?) so that people are used to what they see. Use what they are familiar with, make it intuitive. 

... Never use outlook at home ...

Accessibility, Responsive: UI concepts born out of the web.

Always have access to the source code: example: grid lib, want to restyle, need to request the change from vendor. Can't reach into code and override manually. The web is open.

What do you wish you had known before getting into JS? https://news.ycombinator.com/item?id=17466391










