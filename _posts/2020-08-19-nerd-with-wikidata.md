---
layout: post
title:  "Named Entity Recognition and Disambiguation"
excerpt: My take on NERD with the help of Wikidata
---


### Motivation

Named Entity Recognition and Disambiguation is a challenge in query understading. Here are a couple of examples in case you haven’t heard of NERD.

- black cat: A short horror story by Edgar Poe `||` a manga by Kentaro Yabuki `||` a dark feline
- harry potter: A book series `||` a film series `||` the character `||` [a journalist ;)](https://en.wikipedia.org/wiki/Harry_Potter_(journalist))
- prince: A son of a king `||` A musician

A lot of this is based on the context around the word, which I am aiming to solve for a very short uncased text. Sometimes NLP tools relies on capitalization to detect entities. Remember the last time you capitalize words when typing to Google? I don't.
The lack of context in a short query is also a challenge.

### Demo
[read `harry potter` vs watch `harry potter`?](http://142.93.230.57/)

### Tech stuff

#### Software
- FLAIR for POS
- Wikidata for knowledge base
- Docker compose for deploying
- ReactJS for front end

#### Hardware
- 2GB Ram
- 1 shared CPU

Here I wanted to limit the hardware to find the leanest solution.
