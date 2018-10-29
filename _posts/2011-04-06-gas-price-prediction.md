---
tags: knowledge-graph
comments: false
title:  "News to knowledge graph to prediction"
excerpt: News article can influence stock market, or any market that perform on similar basis. In this paper we aim to create a knowledge graph of linked events and apply to financial series prediction
date:   2018-10-22 22:00:00
---

# Abstract

Gas market is one type of commodities markets. While most of them are not sensitive with news, gas market have become more financialized, making anincrement in their sensitivity to both macroeconomic news and surprise interestrate changes (Roache and Rossi, 2009). In fact, nowadays they follows sameoperation with stock market, which is known for its sensitivity toward news.Finding sentimental meaning and creating knowledge graph from raw textattracts many works. Statistical method like TF-IDF, Bags of Words can serveas a feature for raw text but they cannot capture the semantic behind.
The potential contribution of this paper is
- Build the knowledge graph Learning the semantic from this knowledge graph.
- Use them as a feature for prediction

# Experiment

## Data Description
The database used in this work consists of articles from The New York Times. Each news article consists of its headline, abstract, lead paragraph and publishing date. The publishing date is used to allign with the corresponding price in the financial series. The price series from Future and Spot Market is also included, graciously provided by Bayer AG.

Data cover the period from October 20, 2006 to September 31, 2018

The data is split into a series of windows, each has the length of 20. The stride of the window is 7. Target is the price in three days after each window.  We are currently using Glove embedding to convert the abstract of the news into vector.

Loss is Mean Square Error
## Training result
![Legend](/assets/legend.JPG)
<img src="/assets/train_acc.JPG">
<img src="/assets/val_acc.JPG">

# Proposing next steps
Next step:
- Detect entities and verb to form a knowledge graph
- Link interlinked news together
- Make a knowledge graph
- Use knowledge graph as a feature for prediction

# Reference
Roache, Shaun K and Marco Rossi (2009).The Effects of Economic News onCommodity Prices
