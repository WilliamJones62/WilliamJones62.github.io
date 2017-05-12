---
layout: post
title:  I needed Closures
date:   2017-05-12 02:21:52 +0000
---


I had a code challenge this week. The basic logic was straightforward enough. A warehouse has shelves. Each shelf has only one type of item. The higher the shelf number the further away it is so the longer it takes to pick an item. So the most picked item should be on the first shelf, and so on. Based on the numbers of the various items picked on the previous day I would sort the items in descending count order and display a list of shelves starting at 1 with the most picked item and so on. Easy peasy. 

However the code needed to be in JavaScript, and the previous days orders were stored as a variable, within a function that returned the variable, within a function, in a seperate JS file that could not be edited. I have been working on Angular JS projects for the past 4 months so my vanilla JS was a bit hazy. I knew that scope always went down, so if a variable is defined in a scope 'bubble' all the lower level scope bubbles within it have access to that variable, but all the upper level scope bubbles could not "see" the variable. A very simple rule. So how was I supposed to get access to yesterday's data because it is buried in a function?

I blew the code challenge because I don't know JS well enough. After asking around I was told about a book (actually a series of books) appropriately called 'You don't know JS' that can be found on Github (https://github.com/getify/You-Dont-Know-JS/tree/master/scope%20%26%20closures). In it I learned all about closures. This topic is not covered by the Learn curriculum, but it is one of the most powerful features of JS. Closure means that a function is able to remember and access its scope even when that function is executing outside of its scope. So all I needed to do to access yesterday's data was to set a variable equal to the value returned from the execution of the function within the function, for example like this,   

var yesterday = orderRepo.getYesterdaysOrders();

Simple really, but most things are when you know what to do. 

I really hope I get another chance to show that I understand concept of closures in JS. It really is something every JS programmer needs to know. It is the difference between a junior programmer and real developer and it is used in almost every JS program that is worth running.

