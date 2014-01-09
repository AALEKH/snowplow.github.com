---
layout: section
category: services
title: Web and event analytics
description: We help clients use their Snowplow and other data to quickly answer business questions and drive decision-making
weight: 3
---

# Web and event analytics

We help you use your customer, catalogue and web analytics data to drive platform development and marketing decisions. 

Learn more about our approach to analytics projects below:

1. [Context](#context)
2. [Approach](#approach)
3. [Project output](#output)
4. [Examples of our work](#examples)
5. [Learn more](#learn-more)


<a name="context"><h2>1. Context</h2></a>

The profliferation of data (especially customer data) means there are more opportunities to use it to make the right platform development and marketing decisions.

However, there are often barriers to using data to drive decision making:

* **Data infrastructure**. Few companies have gone through the expensive process of designing and implementing a customer-centric data warehouse, with all the  data transformations enable analysts to query across multiple data sets without programming expertise. Even in companies that have this infrstructure, web analytics data (and other digital data sources e.g. social media) typically lives outside of it
* **Technical skills shortage**. In the absense of a clean data warehouse that brings together all the relevant customer data sources, programming expertise is required to perform the necessary ETL and data crunching
* **Analytic skills shortage**. Even with the relevant technical expertise, significant analytic work is required to turn web analytics and other customer data into a meaningful picture of a customer-base, and then use that knowledge to inform decision making. That analytic process encompasses refining commercial decisions down to specific questions that can be tested with data, identifying the relevant data sources before designing and executing the analyses
 

<a name="approach"><h2>2. Our approach</h2></a>

1. Work with the client to **refine the business decision / question** into a subset of discrete questions that can be addressed in a data-driven way
2. In parallel with the above, **audit all available data sources**
3. **Design and execute the analysis**. Our experience in transforming and joining data sets and familiarity with a wide range of big-data ETL tools means we are able to do this quickly
4. **Pull the analyses together** into a coherent powerpoint deck that addresses the business question head on
5. **Present and iterate the findings with the client**, drawing on client knowledge of their customer-base not captured in the data to colour the analyses


<a name="output"><h2>3. Project output</h2></a>

The primary output of any analytics project is a Powerpoint deck that directly addresses the business question posed, and weaves the different analyses performed into a coherent narrative in support of a specific recommendation for the client.

Some illustrateive analyses from past projects are shown below, to give a flavour of the analyses we produce.


<a name="examples"><h2>4. Examples</h2></a>

### Example consumer analytics: engagement levels over time

A Snowplow client wanted to understand how their user engagement levels were changing over time. One of the measures we experimented with using as a proxy for engagement was the number of days per month that each user that month had logged in for. We then compared the distribution of users each month by the number of days they had logged in that month:

![example-user-engagement-over-time-relative][engagement-graph-1]

A large fraction of users (almost half of them) had only logged in once per month. A large proportion of them represented drive-by-traffic that never returned to the site. Understanding what events happen on that initial customer journey, to turn a "drive by visitor" into a "signed up user" was critical to driving sustained growth for the business over time.

The graph suggested that the fraction of drive by traffic had increased over time, and that as a consequance, overall engagement levels had dropped, since April 2010. It was important to understand whether existin gusers were getting less engaged (which would indicate a long-term, structural problem with the business) or the company was getting better at driving new users to the site, and that these user's inexperience with the site was what was driving down the overall average for engagement.

![example-user-engagement-over-time-absolute][engagement-graph-2]

A look at the absolute number of users in each category showed that it was, indeed, the large number of new users that was driving down the average. Further analysis was then conducted to compare what happened on the user journeys for new users who went on to return to the site with those that did not, to understand what were the events on that journey that were predictive of a user returning. Encouraging these events became a platform development priority.

### Example catalogue and platform analysis: conversion rate by product

The following graph was part of a catalogue analysis performed for an online retailer with a diverse set of more than 5000 SKUs across multiple categories.

![example-catalogue-analysis][product-performance-example]

In the above graph, each circle represents a particular SKU. The size of the circle represents the revenue made through selling it in 2011. The position along the X-axis reflects the number of page views for that product in 2011, whilst the position against the Y-axis reflects the number of times the item was purchases that same year. Hence, the location of the item reveals both it's popularity (in terms of views and purchases) AND how highly converting it is. (With higher converting products appearing further up the Y-axis than along the X, and lower converting products appearing further along the X-axis than up the Y-axis). Also note that *only* the top 1000 products were plotted in this graph, for clarity.

The analysis revealed a number of commercially significant findings:

* The number of page views varies dramatically by SKU. Some variation is always expected, as some products are always going to be more popular than others. However, an analysis over time revealed that the variation increased *faster* than the range. Further, an analysis within each category showed that the top 5 products in each category enjoyed 90% of the page views. This was because navigating between products within each category was especially clunky. (Especially in categories with lots of items.) The site lacked any recommendation functionality, or the ability to allow users to browse within category by theme. As a results, users on typical journies gave up on shopping after visiting less than five products in each category, whether or not they found something they liked to buy.
* The above insight was used to justify an overhaul in the ecommerce platform used, to one that enabled much more flexibility to the client's development team to create multiple routes for users to browse within categories. (And category-specific journies.)
* The conversion rate varied widely between products. Further analysis suggestesd this was **not** related to product pricing. (Conversion rates did not change for specific products if pricing promotions were used.) Rather, it the site template was better used to preview certain categories of products than others. (Conversion rates varied by product categories as a whole, rather than by individual product.) Again, this was used to justify investing in a new ecommerce platform that allowed for more flexible templating between product categories.
* The potential upside from raising conversion rates for poorly converting categories was enormous. In particular, some of the lower converting products were still generating a significant share of overall revenue, in spite of their low conversion rates. Just raising these to be in line with the average across all products would raise overall revenue by more than 15%. 

Note: the above graph was produced using two data sets exported out of Google Analytics and joined together. (Ecomm sales data and page view data.) A better two metrics to plot on the X-axis and Y-axis would be "unique users who viewed page" and "unique users who bought the product". This is possible with Snowplow data, but not with data exported from GA.


<a name="learn-more"><h2>Sounds interesting?</h2></a>

[Get in touch] [get-in-touch] with the Snowplow team to discuss your project. 

[engagement-graph-1]: img/user-dist-by-days-used-service-by-month-perc-breakdown.jpg
[engagement-graph-2]: img/user-dist-by-days-used-service-by-month-actual-figs.jpg
[product-performance-example]: img/pvs-by-unique-purchaes-by-product-2011.jpg
[rate-card]: rate-card.html
[get-in-touch]: /about/index.html
[reporting]: reporting.html
[implementation]: implementation.html
[custom-dev]: custom-development.html
