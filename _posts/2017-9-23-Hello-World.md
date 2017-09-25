---
layout: post
title: First Data Science Project at Metis
---

This Monday, I started my first week of this intense yet exciting 12-week Data Science Bootcamp with Metis. 
Right away, we were divided into group of 3 to start working on our first project which will be due in 4 days applying the knowledge/tools we just learned. The objective of the project was to make recommendation to a hypothetical client "Women Tech, Women Yes" on how they should allocate their volunteers for their upcoming fund raising event, the WTWY Gala, so that they could optimize collection of signatures and gala attendance.

Since the gala will be hold early summer next year, we retrieved published data from New York City Metro Transit Authority data in May 2017 to minimize any noise that could be introduced by seasonal disturbance. The raw data from MTA record the cumulative counts of entries/exits every 4 hours on a turnstile level. We first process the data to show the number of entries/exits in every 4 hours time period. When we looked at the data, we noticed there are a lot of big outliers as shown in the graph below. I discovered that these were caused by regular device reset and unexpected malfunction. After setting up threshold and eliminating these outliers, our data look much more reasonable. 

![alt text](https://github.com/daphnezht/sea17_ds2/blob/master/projects/01-benson/DataCleaning.png, "Data Cleaning")

Next step,  
