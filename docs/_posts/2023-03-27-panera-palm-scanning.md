---
layout: single
title:  "Panera Palm Scanning"
author: mauricio
tags:
  - privacy
categories:
  - blog
header:
  overlay_image: /assets/images/2023/PalmVeins-sm.png
  caption: "Photo credit: Mauricio Tavares, Privacy Test Driver"
excerpt: "Is not having to use your wallet worth surrendering your biometric data?"
---

Panera Bread will start using AWS-based palm scanning as a convenient way to pay for your orders.


Panera Bread 
[started to deploy Amazon-based Palm scanning](https://www.aboutamazon.com/news/retail/introducing-amazon-one-palm-payment-at-panera) 
for payments and loyalty rewards in two locations in the St. Louis area. The reason for using this biometric technology is a 
[frictionless, personalized, and convenient service](https://www.panerabread.com/en-us/press/press-room/panera-continues-loyalty-innovation-with-amazon-one.html): 
instead of its customers having to be inconvenienced with grabbing their wallet 
or phone to pay for their order, all they have to do is hover their hand over 
the sensor and the order it processed and their *MyPanera Rewards* are updated. 
On the top of that, if they hover their hand as they get in, they are greeted 
by name by the Panera associates.

According to Amazon, it scans the shape of your hand and the shape of the 
veins inside it. 
Palm vein pattern recognition is considered a reliable biometric 
identification method since it is unique to a person and does not change much 
with age.

Panera and Amazon claim this technology is much more privacy conscious than other biometric solutions such as face recognition because, according to them, you cannot identify people from looking at the image of their palm.

Well, that reasoning has a few issues:
1. To use the *convenient palm scanning*, customers have to sign up with 
[Amazon One](https://one.amazon.com/), 
the Amazon payment system, which ties their palm print with:
   * Amazon account
   * Mobile number
   * Credit or debit card

    In turn this is tied to their *MyPanera* account. For this to work, palm scanning must be enough to identify customers so Panera can submit the right bill to the right person.
2. Panera also states the data is kept private because it is not stored in Panera computers. While this is correct, it is stored in Amazon computers. There is no nationwide privacy regulation in the United States blocking the tech giant from sharing this information with its partners. The closest regulation limiting the acquisition and sharing of this kind of data is Illinois Biometric Information Privacy Act (BIPA).
1. The main reasoning behind their privacy claim is that it cannot be scanned from a distance. However, this is still biometric data, which is considered personal data under GDPR, CCPA, and BIPA.
1. If it does scan your veins, it can be used to identify vascular problems. In other words, it can collect medical data. As neither Amazon or Panera are medical institutions, they are not restricted by HIPAA from selling/processing this information.

Amazon did say if users submit a request, it will delete their personal information it already collected.

We believe there is no reason for you to allow Panera and Amazon to connect your biometric data. With that said, given this is an opt-in service, 
it is up to you to decide if the convenience outweighs surrendering your 
personal information. 
