
---
layout: post
title: Can Artificial Intelligence write a better booking than 50 Shades of Grey?
date: 2017-03-28
author: jason
comments: true
categories: [text mining, artificial intelligence, machine learning]
---
# Can Artificial Intelligence write a better book than 50 Shades of Grey?

### **Quick Summary**

For all interested writers, authors and creative writing types…. I think it’s fairly safe to assume you’re safe for the time being.

### **Can AI Write Me a Book?**

First of all, this isn’t really about code it’s just about process. So there are no juicy code snippets or scripts to get all hot under the collar about. This whole episode started out with a couple of questions.

1. **_Could AI write a novel or a novella of a quality that it could be entered into a writing competition?_**

2. **_Is it possible to make 50 Shades of Grey readable?_**

<!--more-->

So before my usual working day I downloaded some recurrent neural network code, installed Tensor Flow and trained it on Shakespeare and left the laptop alone to do it’s thing. Yup, training takes a long time, in my case it was eight hours on a commodity Toshiba C70D laptop running Ubuntu. If you want to read more about RNN’s then there’s an [excellent explanation here](http://karpathy.github.io/2015/05/21/rnn-effectiveness/). Generating samples of text generated from the RNN is a doddle….. takes seconds.

### **That Flipping Book.**

So, rinse and repeat with some different text. How about 161,528 words of *that* book. Now, I have a confession I’ve never read that book, or in fact novels, for some reason my brain is firmly planted in non-fiction. Now I’m wondering if I can get AI to write me an O’Reilly book…. wonder what animal I’d get?

Another eight hours pass, overnight this time.

So how quick is it to generate 500 words of AI driven wordery? No time at all it seems.  In fact with some simple bash scripting I can write an 11,500 word novella in under two minutes, on a cheap laptop. I shall be rich after all!

### **Not So Fast**

While the output was, well okay, it needs A LOT OF WORK to make it actually work on a human readable level. The main reason is in the training, if you look at that book it trundles in at 900k long in text file length, for training that’s way too small. In the samples the AI would get stuck in a look at repeat the same phrases over and over. Sometimes it would actually add to the paragraph, most times it repeated so often it didn’t make sense.

*"He looks so remorseful, and in the same color as the crowd arrives and in my apartment. The thought is crippling. But and I don’t want to go to me that I want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to him — and I can tell him about 17 miles a deal."*

The only thing I can think of that came close was [Adrian Belew’s repetitive shouting](https://www.youtube.com/watch?v=JmvA7oWGb40) of "I repeat myself when under stress, I repeat myself when under stress….." (Warning: Youtube link contains King Crimson and a Chapman Stick).

Regardless, part of me thinks that’s naff, part of me thinks that’s rather cool, AI did that. So in theory and with a little cleaning up it’s possible to craft something.

### **What About Topic and Flow?**

This is the thing with creative text, it has characters, themes and a story flow. What I’ve done so far doesn’t address any of that and that’s where everything falls flat on it’s bum for AI. Without some hefty topic wrangling it’s going to be difficult to craft something that’s actually going to flow and make sense.

My favourite book on text mining by a country mile is not one that has tons of code in it, it’s [The Bestseller Code](http://amzn.to/2k9FV9z) by Jodie Archer and Matthew Jockers. It’s a good attempt, while by their admission could be improved, investigation using multivariate analysis, NLP and other text mining tools to see if there were patterns in the best seller list.

![image alt text]({{ site.url }}/assets/images/posts/image_0.png)

Topic is important, that goes without saying. My AI version has no plot line whatsoever as it plainly isn’t told of such matters, if you want to know more about plot lines then there are [the seven basic plot lines](http://tvtropes.org/pmwiki/pmwiki.php/Literature/TheSevenBasicPlots?from=Main.TheSevenBasicPlots) that are widely used. Baking those plot lines to an AI will take work.

The more text you generate the worse it’s going to be to get a basic plot going. A way to get the AI to focus on generating certain aspects of the story over a timeline would be beneficial but hard to do. Once again though, nothing is impossible.

### **An Industry Of Authorship, Automated?**

The future automation of all things literature I think is a long way off. Though, let’s look at this from a 30,000ft view. I can generate an eleven thousand word book, while ropey, showing some promise if only needing an editor to sort the wording out.

API’s that exist now, well I could pick of for words to form a title. "rules are a hostile anthem" came out…. one Google Image Search for creative commons photos….

![image alt text]({{ site.url }}/assets/images/posts/image_1.png)

And automatically pick an image that fits a certain AI criteria. No text… pass that on to an overlay of the title of the book and the author’s name, "Alan Inglis" (geddit A.I.) and package that up in a Kindle format (that can be automated too) and off it goes to an Amazon account.

*I did check on Alan Inglis, there are no authors of that name but, rather ironically, one within clinical neurosciences….. I should write an algorithm to create a surname that doesn’t exist really. I just guessed this one out.

### **Perhaps Not Fiction Then….**

Perhaps not, but with texts that tend to take the same form it could be easy to create fairly accurate drafts which require some form of editorial gaze afterwards. News reports, Invest NI jobs created press releases, term sheets and even business plans. Yup I think there’s sufficient scope for something to happen. I don’t think you’ll replace them human element but then again you don’t really want to.

### **Back, To Answer My Original Question**

So, could my AI submit something to writing competition? Perhaps it could if it were less than 10,000 words. With enough corpus text it would be possible to do something of a quality that could be considered readable. Would a judge notice it as AI writing, who knows. There are some bits with the samples I’ve generated that are quite interesting, it looks like there’s heart in the prose but it’s simply not true.

I think the Alan Inglis’s of this world are safe for the time being….. I suppose I should go and read [The Circle by Dave Eggers](http://amzn.to/2jQJVuA) to see what my future holds.

### By Jason Bell. 

Jason may not (yet) have coaxed a best-selling book out of a machine, but, using the old fashioned method of writing it himself,  was the author of *Machine Learning: Hands On For Developers and Technical Professionals*.  At Mastodon C he specialises in high volume data workflows and pipelines.

