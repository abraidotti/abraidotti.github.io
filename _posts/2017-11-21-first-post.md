---
layout: post
title: Gotta start somewhere. I'm starting with Sinatra.
---

I'm currently a student at [NYCDA's](http://nycda.com) three-month Web Development Intensive bootcamp. There are about 18 other people in my cohort.

Our latest assignment is to use the Sinatra framework to create a message board-style app.

My costudents Chris, George, and I finished ours up a day early. Chris and George are great. The class took about a week to get through Sinatra routing basics, but George clued me in to using embedded Ruby (aka ERB) with dexterity.
Let's take a look at the first example:

![msg maker nav code](/img/2017-11-21.msg-maker-nav.png "Msg Maker Nav code")

As you can see in the commentary, George and I made some dynamically-updating buttons all in ERB, without using an javascript. Here's a video of the nav in action.

<div style="width:100%;height:0;padding-bottom:63%;position:relative;"><iframe src="https://giphy.com/embed/xUNd9LkX4s4Myu24GQ" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div>

Sure, we could have designed a functional, maybe even elegant, solution with some Javascript event listeners, but George's minimal approach worked even better. It takes up fewer lines of code, less processing power, and it's all there in one file.
