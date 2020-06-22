---
tags: knowledge-graph
comments: false
title:  "News to knowledge graph to prediction"
excerpt: News article can influence stock market, or any market that perform on similar basis. In this paper we aim to create a knowledge graph of linked events and apply to financial series prediction
date:   2018-10-22 22:00:00
mathjax: true
---

<mark> This is an ongoing document and will be updated in weekly basis

# Abstract

Gas market is one type of commodities markets. Unlike most of them, gas market are more and more sensitive to news (Roache and Rossi, 2009). In fact, their sensitivity are getting to the same level of  stock market. Therefore, integrating sentimental meaning and creating a knowledge graph from news can serve as a feature in market prediction. 
The potential contribution of this paper is
- Build the knowledge graph 
- Learning the semantic from this knowledge graph.
- Use them as a feature for prediction

# Introduction

# Related works

# Experiment

## Data curation
subsection{Data Description}

Training data includes price series from Bayer's AG specific suppliers in the GPL and NCG trading hub. News articles are from The New York Times and The Guardian (\citet{nytimes_api, guardian_api}) published
 from October 20, 2006 to November 21, 2013. 
 \subsubsection{The New York Times}
 As The New York Times only allow downloading every news any given month and year without any filtering, we came up with a crude discrimination rule by sections, leaving out Blog, OpEd, Editorial, and keeping news that contains some keywords like 'Energy', 'Natural Gas' or 'Petroleum'. Each news article consists of its headline, abstract, lead paragraph and publishing date.
 \subsubsection{The Guardian}
 The Guardian support search by keywords and section. Articles about natural gas price are categorized into Business section, while events are into World section.
\subsection{Baselines}
We investigate the effect of news on the Future and Sport Market. Concretely let $X$ be the word embedding of news headline, $Y \in \{0,1\}$ in which 0 means equal or decreasing price in comparison with the previous day, 1 otherwise, $n$ the news published day, $n+k$ the next $k$ trading day.  A Chained CRF is used in combination with the word embedding vector to classify $Y_{n+k}$ from $X_n$


% Can be some weird stuffs: Who owns the artic, nytimes


\begin{table}[]
\begin{tabular}{|l||l|l|l|l|l|l||l|l|l|l|l|l|}
\hline
Data & \multicolumn{6}{|l||}{Future Market} & \multicolumn{6}{l|}{Spot Market} \\
\hline
$k$      & 1 & 2 & 3 & 4 & 5 & 6 & 1 & 2 & 3 & 4 & 5 & 6 \\
\hline
\hline
1st Paragraph & 0.5187 & 0.5317 & 0.5159  & 0.5159  & 0.4957 & 0.5051 & 0.5147 & 0.5073  &  0.5220 & 0.4982  & 0.5018  & 0.4991 \\
Header & 0.5048 & 0.5478 & 0.4378 & 0.5359 & 0.5383 & 0.5383 & 0.5421 & 0.5387 & 0.5286 & 0.5354 & 0.5017 & 0.4662 \\
\hline
\end{tabular}
\caption{Comparison of CRF's performance in different markets at different $k$}
\end{table}
 \citet{RePEc:eee:quaeco:v:50:y:2010:i:3:p:377-385} suggested that headlines are more useful to forecast than contents. Our experiment sees some minor enhancements, but nothing conclusive yet.


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
