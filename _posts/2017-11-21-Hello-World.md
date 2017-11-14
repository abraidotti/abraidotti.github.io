---
layout: post
title: Gotta start somewhere. I'm starting with Sinatra.
---

I'm currently a student at [NYCDA's](http://nycda.com) three-month Web Development Intensive bootcamp. There are about 18 other people in my cohort.

Our latest assignment is to use the Sinatra framework to create a message board-style app.

My costudents Chris, George, and I finished ours up a day early. Chris and George are great. The class took about a week to get through Sinatra routing basics, but George clued me in to using embedded Ruby (aka ERB) with dexterity.
Let's take a look at the first example:

`<nav>
      <a class = "left" href="/">home</a>
      <!-- first check the user's login status -->
      <% if !session[:login] %>
        <!-- if user is not logged in, display a "login" button: -->
        <!-- otherwise, display "logout" -->
        <a class = "left" href="<%= current_user == nil ? '/login' : '/logout' %>">
        <%= current_user == nil ? 'login' : 'logout' %>
        </a>
        <!-- and if the user is logged in, display a "view my profile" button -->
        <% if current_user != nil && !session[:in_profile_page] %>
          <a class="right" href="/profile/show/<%= current_user.id %>">
            View My Profile
          </a>
        <% end %>
      <% end %>
    </nav>`

As you can see in the commentary, George made some dynamically-updating buttons all in ERB, without using an javascript. I was impressed. Here's a video of the nav in action.

<iframe width="560" height="315" src="https://www.youtube.com/embed/3-6Oi7x-Lx4" frameborder="0" gesture="media" allowfullscreen></iframe>
