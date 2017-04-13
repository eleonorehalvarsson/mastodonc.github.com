---
layout: post
title: Can Artificial Intelligence write a better book than 50 Shades of Grey?
date: 2017-04-13
author: jason
comments: true
categories: [text mining, artificial intelligence, machine learning]
---

Spoiler alert. All you writers, authors and creative writing types who may be worrying about AI, rest easy, you’re safe. For a while...

<!--more-->

### **Can AI Write Me a Book?**

First of all, this isn’t really about coding it’s about process. So, in this article, there are no juicy bits of code or scripts to get all hot under the collar about.  

This whole episode started out with a couple of questions.

1. **_Could AI write a novel or a novella of a quality that it could be entered into a writing competition?_**

2. **_Is it possible to make 50 Shades of Grey readable?_**

So, before my usual working day I downloaded some RNN code (RNNs, short for recurrent neural networks, are a way to help computers solve problems in a similar way to the human brain). I then installed Tensor Flow (a tool that enables computers to learn), and trained it on Shakespeare (an up and coming Engish playwright and poet). Then, left the laptop alone to do it’s thing. Yup, training takes a long time, in my case it was eight hours on a commodity Toshiba C70D laptop running Ubuntu. If you want to read more about RNN’s then there’s an [excellent explanation here](http://karpathy.github.io/2015/05/21/rnn-effectiveness/). Generating samples of text generated from the RNN is a doddle, it takes seconds.

### **That Flipping Book.**

The next step was to rinse and repeat with some different text. How about 161,528 words of *that* book (50 Shades of Grey - for those of you not paying attention). I have a confession I’ve never read *that* book, or in fact many novels. For some reason my brain is firmly planted in non-fiction.  So, now I’m wondering if I can get an AI to write me an O’Reilly published book. And, if it can, if it could even choose for itself a cool picture of an animal for the front cover.

Another eight hours pass, overnight this time.

Finally, how quick is it to then generate 500 words of AI driven wordery? No time at all it seems.  In fact with some simple bash scripting it's written a 11,500 word novella in under two minutes, on a cheap laptop. I shall be rich after all!

### **Not So Fast**

While the output was, well okay, it needs A LOT OF WORK to make it actually work on a human readable level. The main reason is in the training you need to do, if you look at *that* book  it trundles in at a 900k text file, for those of you familiar with what it takes to train an AI, that’s way too small. In the samples the AI created it would get stuck in a loop, and repeat the same phrases over and over. Sometimes it would actually add to the paragraph, most times it repeated so often it didn’t make sense.  Here's some of the sample text, so you can see what I mean:

*"He looks so remorseful, and in the same color as the crowd arrives and in my apartment. The thought is crippling. But and I don’t want to go to me that I want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to you. I don’t want to be beholden to him — and I can tell him about 17 miles a deal."*

The only real life bit of art I can think of that comes close to that is [Adrian Belew’s repetitive shouting](https://www.youtube.com/watch?v=JmvA7oWGb40) of "I repeat myself when under stress, I repeat myself when under stress….." 

Regardless, part of me thinks ""that’s not great"", but part of me thinks ""that’s rather cool, AI did that."" So, in theory and with a little cleaning up, it is indeed possible to craft something.

### **What About Topic and Flow?**

That said, the thing with creative text is that it has characters, themes and a story flow. What I’ve done so far doesn’t address any of that and that’s where everything falls flat for AI. Without some hefty topic wrangling it’s going to be difficult to craft something that’s actually going to flow and make sense.

My favourite book on text mining is not one that has tons of code in it, it’s [The Bestseller Code](http://amzn.to/2k9FV9z) by Jodie Archer and Matthew Jockers. It’s a good attempt (which by their admission could be improved) at investigating if there are patterns in the best seller list that reveal the secrets to writing a best-seller.  For the record they used multivariate analysis, NLP and other text mining tools.

![image alt text](/assets/images/AIbook_0.jpg)

Topic is important, that goes without saying. My AI novel has no plot line whatsoever. But that's not its fault because it hasn’t be taught about such lofty matters. For the record there are (according to this article at least) [seven basic plot lines](http://tvtropes.org/pmwiki/pmwiki.php/Literature/TheSevenBasicPlots?from=Main.TheSevenBasicPlots) that are widely used in novels. But even teaching a few of those plot lines to an AI will take work.

The more text you generate the harder it will be to get a basic plot going. A way to get the AI to focus on generating certain aspects of the story over a timeline would be beneficial, but again hard to do. Nothing however is impossible.

### **An Industry Of Authorship, Automated?**

The future automation of all things literature is therefore a long way off. Though, let’s look at this from a 30,000ft view. I can already generate an eleven thousand word book, which, while ropey, shows some promise, and not far off only needing an decent editor to sort it out.

So here's how it could work in practice.  We can pick off existing APIs for words to form a title. Doing that produced "rules are a hostile anthem", a pretty decent title.  Add in Google Image Search for creative commons photos….

![image alt text](/assets/images/Googlepics_1.png)

Then automatically pick an image that fits a certain AI criteria.  Pass that on to an overlay of the title of the book and the author’s name, "Alan Inglis" (geddit? A.I.?) and package that up in a Kindle format (that can be automated too). And off it goes to an Amazon account.

(I did check on Alan Inglis, there are no fiction authors of that name but, rather ironically, one within clinical neurosciences. I should write an algorithm to create a surname that doesn’t exist, but on this occasion I just guessed this one out.)

### **Perhaps Not Fiction Then….**

Perhaps fiction, with it's complicated plots, themes and characters isn't the best domain for Alan Inglis and other budding AI authors.  But with texts that tend to take a similar structured and form it could be easy to create fairly accurate drafts, which would then just require some form of editorial gaze afterwards.  News reports, press releases, term sheets and even business plans. Yup I think there’s sufficient scope for something to happen. I don’t think you’ll replace the human element entirely, but then again I don’t really want to.

### **To Answer My Original Question**

So, could my AI submit something to a writing competition? Perhaps it could if it were less than 10,000 words. With enough corpus text to train the machine it would be possible to do something of a quality that could be considered readable. Would a judge notice it as an AI writer?  Who knows? There are some bits in the samples I’ve generated that are quite interesting.  And it looks like there’s a human heart in parts of the prose, even if that's simply not true.

The (real) Alan Inglis’s of this world are safe. For the time being.


#### Article by Jason Bell. 

Jason may not (yet) have coaxed a best-selling book out of a machine, but, using the old fashioned method of writing it himself,  was the author of *Machine Learning: Hands On For Developers and Technical Professionals*.  At Mastodon C he specialises in high volume data workflows and pipelines.

