---
tags: knowledge-graph
comments: false
title:  "News to knowledge graph to prediction"
excerpt: News article can influence stock market, or any market that perform on similar basis. In this paper we aim to create a knowledge graph of linked events and apply to financial series prediction
date:   2018-10-22 22:00:00
---

# Abstract

Gas market is one type of commodities markets. Unlike most of them, gas market are more and more sensitive to news (Roache and Rossi, 2009). In fact, their sensitivity are getting to the same level of  stock market. Therefore, integrating sentimental meaning and creating a knowledge graph from news can serve as a feature in market prediction. 
The potential contribution of this paper is
- Build the knowledge graph 
- Learning the semantic from this knowledge graph.
- Use them as a feature for prediction

# Experiment

## Data curation
The database used in this work consists of articles from The New York Times and the Guardian. 

<mark>NEW

News are then manually compared with Quarterly Reports on Gas Market of European Council to see if they have covered all of the information in these reports. Normally important elements that affect spot market are:
- Dispute, mainly between Russia and Ukraine
- Weather conditions
- The economic slowdown (GDP can be an indicators)
- Demand of power generators, this depends on demand of electricity  
- Liquidity (Platts service, cost money)
- Import amounts, corellates with GDP, can download one in two

What affects electricity demands
- To be added

Elements that affect future market
- The economic slowdown

<mark>END

Each news article consists of its headline, abstract, lead paragraph and publishing date. The publishing date is used to allign with the corresponding price in the financial series. The price series from Future and Spot Market is also included, graciously provided by Bayer AG.

Data cover the period from October 20, 2006 to September 31, 2018

The data is split into a series of windows, each has the length of 20. The stride of the window is 7. Target is the price in three days after each window.  We are currently using Glove embedding to convert the abstract of the news into vector.

Loss function being used is Mean Square Error

## Knowledge graph first idea
<mark>NEW
An interlinked event for the knowledge graph
Event: Dispute between Russia and Ukraine in 2009 that leads to 13 days Natural gas cut off in Europe. 
- October 2008: Ukrainian and Russian Prime Ministers signed a deal that. 
    - Appoint Naftogaz as the only importer of Ukraine. 
    - Raise import prices and transit taxes based on mutual agreement. 
- November 2008: Naftogas (UA) and Gazprom (RU) disputed in transit fee and import price. 
- … many pointing fingers and settlements in between. 
- December 19: Gazprom stated that no supply contract could be signed for 2009. 
- January 7: deliveries to Europe completely cut off. 
… EU Commitee took action. 
- January 22: Gas flows to Europe return to normal level. 

<mark>END
## Training result
![Legend](/assets/legend.JPG)
<img src="/assets/train_acc.JPG">
<img src="/assets/val_acc.JPG">

# Proposing next steps

<mark> NEW

Next step:
- Forward email to check taxonomy, if it is CEVO
- Words from news will be map to their taxonomy classes (warns -> advise)
- Link close date, time and entities together
- Prove of knowledge graph (node4j)
- Still no machine learning to this point
<mark> END

# Reference
Roache, Shaun K and Marco Rossi (2009).The Effects of Economic News onCommodity Prices
