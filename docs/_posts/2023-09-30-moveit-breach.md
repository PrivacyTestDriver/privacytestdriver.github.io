---
layout: single
title:  "MOVEit breach and Baby Records"
author: mauricio
tags:
  - privacy
categories:
  - blog
---
The title of this blog entry does sound like clickbait, 
but it is surprisingly accurate.
On 25 September 2023, Canada's Better Outcomes Registry & Network (BORN) 
[officially announced](https://www.bornontario.ca/en/news/cybersecurity-incident-moveit.aspx) 
it has joined more than 2000 organizations affected by the 
[MOVEit](https://www.ipswitch.com/moveit)'s vunerability. 
According to [BORN Ontario](https://www.bornincident.ca/),
that translates to the personal and health records 
-- names, addresses, health card numbers, test lab results,
fertility, pregnancy, newborn and child healthcare -- of 
3.4 million people, 2 million of which being newborns born in Ontario between 
January 2010 and May 2023 -- were compromised.

The sequence of events looks like a replay of our discussion on
[Wordpress plugins]({% post_url 2023-05-27-wordpress-and-supply-chain  %}) 
and the importance of maintaining a healthy supply chain:
vendor finds vulnerability, publishes patch, and customers do not apply it.
On 31 May 2023 [Progress Software](https://www.progress.com/) disclosed a
vulnerability that affected its MOVEit Transfer and MOVEit Cloud products, and
issued a patch to address that. This vulnerability had a severity rating of 
9.8 out of 10. Further patches were issues on 9 June and 15 June.

Why has these patches not been deployed by the affected organizations which
run MOVEit locally (on premises)?
Unfortunately, some companies have strict patch policies such as only allowing
updates once every quarter or only when they do not affect the deadlines of
the income-generating -- marketing, sales, product development -- groups.

Maintain your supply chain!
