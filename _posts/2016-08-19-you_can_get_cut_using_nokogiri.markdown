---
layout: post
title:  "You can get cut using Nokogiri!"
date:   2016-08-19 18:06:57 +0000
---


I don't know if the hotel website Trivago uses Nokogiri to get the data from the hundreds of websites it claims to search but it must be quite difficult. 

The biggest problem that I have had with Nokogiri is that on complex websites it can be difficult to get a unique identifier for the data you want. For example if a site has 2 tables that have the same div and class and you only want data from the first you can end up with data from the second as well. It would be nice if web page designers gave unique identifiers to each item, but of course they don't. It can take a very complex collection of identifiers (if that is the right word) to get to the data you want, and only the data you want.

That being said Nokogiri is a very useful tool. But like all tools it can be quite dangerous in the wrong hands (like mine).
