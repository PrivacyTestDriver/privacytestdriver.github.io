---
layout: single
title:  "Wordpress and The Dangers of Supply Chain Vulnerabilities"
author: mauricio
tags:
  - privacy
categories:
  - blog
---
One thing we like to talk to our customers about is the importance of
securing their supply chain. Using the chain analogy, no matter how secure and
private aware is your product, it is but the end of a chain of products
supplied by other organizations (be them open source or not) that are put
together in whatever form you specified. This chain is as strong as its
weakest link.

To make this a bit more real, let's talk about a famous software
[Wordpress](https://wordpress.com/)
is possibly the most commonly used web content manager.

There is a running joke about how insecure it is given the mind-boglling
number of vulnerabilities related to it.
Thing is, WordPress by itself is actually quite secure.
The source of vulnerabilites is the plugins, and the top two reasons are

- There are a lot of them.
Some are well written and maintained, others not quite.
People building websites look for plugins based on which task they are
trying to solve and feedback. This feedback most of the time is about how
easy to install and use a given plugin is; just because a plugin is popular
does not mean it is well maintained, specially regarding security.

- Many people deploy these plugins in a
fire-and-forget fashion: they will only check on whether the plugin has
a new update when it crashes or cause the site to crash.
This by far is the largest source of problems: it does not matter how
quickly the developers identify a vulnerability and create a patch to fix it;
if nobody applies it, it is useless. Worse: attackers will now know the patch
has a vulnerability and then will start looking for unpatched sites.

Let's use a real life example to show how bad that can be:
A few days ago we learned that the
WordPress cookie consent plugin named Beautiful Cookie Consent Banner, which
is currently deployed in more than 40,000 locations (you may have a
single deployment being used by multiple websites),
is
[vulnerable to
Unauthenticated Stored Cross-Site Scripting (XSS)](https://www.bleepingcomputer.com/news/security/hackers-target-15m-wordpress-sites-with-cookie-consent-plugin-exploit/). This allows an attacker to send malicious commands to a
vulnerable website (do you remember the 40 thousand locations we mentioned
earlier? That translates to more than **1.5 million websites**) and take over
not only the website but also the computer running it.
Since this is a privacy blog, we need to talk about that angle: once they
compromise the website, they can go after any confidential information --
user data, passwords, credit card info -- available in the website.

This vulnerability has been known since
[January](https://www.pluginvulnerabilities.com/2023/01/31/hacker-might-be-exploiting-unfixed-plugin-vulnerability-that-wpscan-patchstack-and-wordfence-all-claimed-was-fixed/), and has been patched by the developer, but many sites have
yet to apply the patch.

If we go back to our supply chain, the original weak link was the plugin.
That was solved. The next weak link is to ensure the patched plugin is used
in the website. Until that is done, this chain is still very weak.

