---
layout: post
title:  "Regex (if you will pardon the expression)"
date:   2017-06-12 23:23:50 +0000
---


Maybe I am a bit dim (some would say there is no maybe about it) but I didn't really get a good grip on Regular Expression while doing the course. It all seemed a little esoteric. I thought it didn't seem very important to really understand why it did what it did. Perhaps it was because I couldn't see a real need for it. 

I have been learning Java to try and impress a potential employer. Hacker Rank (https://www.hackerrank.com/challenges) has a series of challenges that let you gradually increase your knowledge of Java. One section has to do with Strings. One challenge in this section is to see if a string contains a valid IP address, another to extract an area code from phone numbers in various formats, and yet another to parse some HTML and extract the data between two matching tags. All of these could be achieved by writting some Java code, but it is much easier (and therefore quicker) to write some Regex.

According to the ever accurate Wikipedia 'A regular expression, regex or regexp (sometimes called a rational expression) is, in theoretical computer science and formal language theory, a sequence of characters that define a search pattern. Usually this pattern is then used by string searching algorithms for "find" or "find and replace" operations on strings.' This is all true. You tap in a string of characters and/or metacharacters to create a pattern. Then you use the pattern to find substrings within the string you want to search. The more specific the pattern the more likely it is that the results produced will be accurate. There are a whole host of useful metacharacters that allow such things as short cuts eg \d means integers 0-9, \s meaning all white space charachters and \w meaning all alphanumeric characters. There are metacharacters that allow you to specify repetitions of characters you want to find such as + meaning at least one repetition and {m} where m is an integer indicating the number of repetitions. A pair of the most useful meta characters is (....) where .... is the regex describing the substring you want to capture. This data is stored and can be processed further outside of Regex (as in the area code challenge, or back referenced in Regex as in the HTML challenge.

There is some disagreement about whether Regex should be used to parse HTML (see https://stackoverflow.com/questions/1732348/regex-match-open-tags-except-xhtml-self-contained-tags/1732454#1732454). I think it depends on the HTML source that you are working with.

Anyway there are a lot of great resources for improving your Regex skills. My favorite is regexone.com. In each section it gives a bit of a lesson and a little challege to test you understanding. You can see the effect on the test data of any Regex changes you make immediately. So you can play around with the various metacharacters and see what they do.

So learn Regex is my advice, you will need it.
