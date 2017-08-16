---
layout: post
title: When is Excel Good Enough?
date: 2017-08-16
author: seb
comments: true
categories: [data science, excel]
---


One question that often comes up when we talk to people new to data science is "Why not just use Excel?"  It’s a reasonable question that’s not as easy to answer as you might think, but answering it does go some way to answering a key question anyone planning a data science project needs to consider - what’s the simplest way to get to the results I need?

<!--more-->

Someone with coding experience might be expected to sniff at Excel. Their response may be "well, why *would* you use Excel?" Excel is almost the antithesis of the open source world that much of data science is built around - it’s corporate, closed and (to some minds) clunky.

However, to my mind, there is no inherent reason to choose code (in any language) over Excel. As with many business problems, the most straightforward route to an answer or result is often the best.

So the simple answer to this question is often "if you can do the job in Excel, and you can use Excel, do it in Excel".

<!--HubSpot Call-to-Action Code --><span class="hs-cta-wrapper" id="hs-cta-wrapper-2d5848d9-00d4-4807-8040-ee03471d6f27"><span class="hs-cta-node hs-cta-2d5848d9-00d4-4807-8040-ee03471d6f27" id="hs-cta-2d5848d9-00d4-4807-8040-ee03471d6f27"><!--[if lte IE 8]><div id="hs-cta-ie-element"></div><![endif]--><a href="https://cta-redirect.hubspot.com/cta/redirect/3461032/2d5848d9-00d4-4807-8040-ee03471d6f27"  target="_blank" ><img class="hs-cta-img" id="hs-cta-img-2d5848d9-00d4-4807-8040-ee03471d6f27" style="border-width:0px;" src="https://no-cache.hubspot.com/cta/default/3461032/2d5848d9-00d4-4807-8040-ee03471d6f27.png"  alt="Download a free checklist: Getting a Data Project Started"/></a><!-- end HubSpot Call-to-Action Code -->

But Excel is not always fit for purpose. To make things easier here’s a summary of the key differences between Excel and coding languages commonly used in data science, like Clojure and R. Weighing up the differences should help you decide whether to do a data analysis in Excel or whether it will need coding.

## Pretty Interface Vs. Command prompt

Probably the most obvious difference between Excel and coding is that Excel has an easy to use GUI (graphical user interface - essentially the thing that allows you to point and click your way around). Excel has buttons, help and instructions, and a standardised way of working. The table and cells provide a clear format and structure for data. All of which help you get to grips with the software quickly and make it easier to get started with analysis.

Conversely, to make use of some new functionality in a coding language, you typically need to either test it out until it works or trawl through the, sometimes meaningless, [man pages](https://href.li/?https://en.wikipedia.org/wiki/Man_page). Indeed, this is typically what is most intimidating about coding to people without coding experience.

But this also points to the flexibility of coding over Excel; Excel is limited by its format and the available functions presented to you, whereas the possibilities for coding up your own program/model/tool/etc. are nearly endless.

## Prebuilt functions Vs. Flexibility

One of the great things about open source software is all the libraries and packages out there that have been built by other users, and that can be used and adapted by you to do the job you need to get done. If there is a problem you are trying to solve, it’s likely that someone out there has tried to solve it before.

Excel has inbuilt functions for doing certain calculations or transformations, which can be strung together to make something which can begin to look a little like code. However, because Excel is "closed" software, it is nearly impossible to interrogate these functions, i.e. check the code to see that what they are doing is what you expect them to do

Here’s an example: if you wanted to build your own function which did *x* recursively over a set of data/cells, you may look to a simple function in Excel like SUM, which adds all data points together to give you a total. Under the hood this is doing something similar to what is called a reducer, whereby the function (add/plus/+) is called over and over again across the data points, each time an intermediate value is stored and added to the next data point, which all results in a single output. It is the looping/reducing aspect of the function that we want to get at, but that is not possible in Excel, whilst it is probably one of the more important aspects of data science coding, especially when dealing with big data.

Conversely, there are many functions in Excel (like SUM) which just work as you expect them to. This may not always be the case in your language of choice, and without understanding the intricacies of the language, or potentially the mathematics, it may not be straightforward to code up an equivalent function in that language.

## Tables Vs. Everything else…

As alluded to in the previous section, Excel is, almost exclusively, designed for use with tabular formatted data. There are more opportunities to use other data structures for more experienced Excel users, but dependent on your language of choice, which do favour specific data structures, there is no limit to how you might want to structure your data (even if it is a plain old table!).

## Medium Vs. Big Data

I’m sure many people working with Excel will have come across a file which overloads Excel, causing it to crash, or take an exorbitant amount of time to open! At Mastodon C we often work with files of this size from local government, which we have come to term "medium" sized data; this is “annoying sized data”, too big for Excel, but not big enough to be considered “big data”.

[As a side note the meaning of the term "Big Data" is difficult to pin down. For the purposes of this article I’ll define “Big Data” as “data large enough, or coming in fast enough that you need to scale your hardware and software to cope with it in a reasonable time”. [This talk](https://skillsmatter.com/skillscasts/7243-expressive-parallel-analytics-with-clojure), from 4:01 on the video, by Henry Garner, has a bit more explanation on what we mean by medium/annoying size data]

In almost all cases your coding language of choice will be able to cope with the data, whatever size you throw at it - small, medium or big. If you’re dealing with real "big data", you should, for example, be looking into [Spark](https://href.li/?https://spark.apache.org/) or [Hadoop](https://href.li/?https://hadoop.apache.org/) or something similar, which will have some sort of package which will work with your language.

N.B. As far as I know Excel doesn’t work with [Amazon Web Services](https://href.li/?https://aws.amazon.com/), but you never know what Microsoft’s up to with [Azure](https://href.li/?https://blogs.office.com/en-us/2016/08/03/announcing-the-general-availability-of-the-microsoft-excel-api-to-expand-the-power-of-office-365/).

## Simplicity Vs. Complexity

Most languages weren’t built from the ground up to be data processing or analysis tools, which, is probably Excel’s main use. This can mean that, once again, you can build whatever you want in your language of choice, however it may be quicker (if not simpler) to process "some" data in Excel.

## The takeaway

When it comes to data, size matters. As does complexity. If you’re dealing with "medium size" or big data you’re going to run into Excel’s limits pretty quickly. Similarly, if your analysis is pretty straightforward, the data size is smallish and you don’t need to get under the hood of the functions you’re using, Excel might be the best place to start.

However over the course of writing this post I’ve also come to realise that although you can build an analysis pipeline in Excel or one or another coding language, these two things are perhaps not really the same thing and subsequently suffer from false similarity. This is also why it is quite hard to answer the question "which one to use?" Although one could use either to find the answer to a problem, the two methods are not always comparable side by side.

The best answer to the question might be the one we started with "it doesn’t really matter what you use as long as you know enough to get the job done efficiently and well".

Understanding the art of the possible is key.  Which also means that if you’re doing a decent amount of data analysis in your job, and pushing the boundaries of Excel, you may need to consider developing some coding skills or finding a friendly data scientist to work with.
