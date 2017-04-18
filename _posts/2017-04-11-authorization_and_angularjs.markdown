---
layout: post
title:  "Authorization and AngularJS"
date:   2017-04-11 08:42:23 -0400
---


I have used Devise and OmniAuth in previous projects but never with a project using Angular. I wanted to include it in my Football Talk app so that users could see each others posts about a game, but could not edit or delete posts that were not theirs. 

I did a lot of google searches and found a lot of blogs about how to use Devise (not OmniAuth) with Angular, but I found them all very confusing (if anybody knows of a blog in easy to read English I would be very interested to read it). In the end I decided to use Devise and OmniAuth as I had done previously and keep it out of the Angular part of my project. This worked well to a point. Sign up, sign on, sign on through Facebook, and sign out all worked as expected. Users can see all the posts for a game, but can only edit and delete their own. However when they attempt to edit or delete another users posts they are prevented but the error messages are not displayed. It's not the end of the world as the functionality is correct, but it is not the best user experience.

I am now looking at Auth0 (Auth0.com) to see if I can use it for authorisations in Angular apps. If it works I may retrofit it to mu Football Talk app. As authorisation is such a fundamental part of so many applications I am surprised that there isn't a standard approach (or Gem) that is available. Maybe there is but I just don't know what it is. If you know please point me in the right direction.
