---
comments: false
excerpt: An overview and reflection of my portfolio
---
### Health hackathon
In 48 hours, my team created E-Prescription, an Android app to remind patients to take their medicine. 

**What I like:** In Vietnam, antibiotics are overused as one does not need a doctor's prescription to buy some. When they forgot to take their medicine, it is common to double the dosage in the next intake. It contributed to Vietnam being among the most overly tolerant antibiotic countries. 

<div align="center" float="left">
<figure>
<img align="left" src="https://cdn.techinasia.com/wp-content/uploads/2013/11/jv-hacking-fest-vietnam-saigon-720x540.jpg" alt="drawing" width="350"/>
  <iframe width="350" height="263" src="https://www.youtube-nocookie.com/embed/2OjyYhaLu5w?start=9" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  <figcaption>In the picture, I am the first from the right, top line. </figcaption>
  <figcaption>In the video, I am  the speaker from 0:09 to 0:17</figcaption>
 </figure>
</div>

[[Our app featured in Tech in Asia](https://www.techinasia.com/jv-hacking-fest-healthcare-hackathon-vietnam)][[Facebook page of the Hackathon](https://www.facebook.com/jvhackingfest/?fref=nf)] 

---

### Industrial robotics software
Pose estimation on a tabletop environment challenge, whose whole dataset consists of two images. My work helped the University of Bonn’s win the EuroC Challenge.

<div align="center">
  <figure>
  <img height="263" src="/assets/nut_train.jpg"/>
  <img height="263" src="/assets/nut_test.jpg"/>
     <figcaption>Definitely the biggest dataset I have worked on. Left: Train data. Right: Test data</figcaption>
 </figure>
</div>

**What I like:** How I adapted when the training data consists of RGBD data of one image and still deliver (Citroën bought our work!)

[[EuroC Challenge](https://web.archive.org/web/20191204203324/http://www.euroc-project.eu/index.php?id=nimbro_manufacturing)][[Paper](\href{https://arxiv.org/abs/2001.04134)]

---

### Rapid road detection
Road detection with 50% faster interpretation speed and retain more than 95% quality. 

<div align="center">
  <figure>
  <img src="/assets/segmented.gif"/>
     <figcaption>Green means another lane or intersected road, pink is the road the car currently on</figcaption>
 </figure>
</div>

**What I like:** My first computer vision project. Seeing the result of the work in the visual form was quite a sensation.

[[Implementation](https://github.com/minhtriet/clockwork-kitti)][[Paper](https://arxiv.org/pdf/2010.15250.pdf)]

---
### Master thesis
Gas price prediction

**What I like:** I stepped away from accepting the model as the black box and tried to wrestle some sense out of it. Below are the ten most influential words to gas price according to my model. It is Table 6 in my paper.

<div align="center">
 
<table>
<thead>
<tr>
<th></th>
<th>2012</th>
<th>2018</th>
</tr>
</thead>
<tbody>
<tr>
<td>1</td>
<td>oil</td>
<td>energy</td>
</tr>
<tr>
<td>2</td>
<td>energy</td>
<td>gas</td>
</tr>
<tr>
<td>3</td>
<td>price</td>
<td>oil</td>
</tr>
<tr>
<td>4</td>
<td>FTSE</td>
<td>China</td>
</tr>
<tr>
<td>5</td>
<td>fall</td>
<td>Trump</td>
</tr>
<tr>
<td>6</td>
<td>shale</td>
<td>trade</td>
</tr>
<tr>
<td>7</td>
<td>power</td>
<td>price</td>
</tr>
<tr>
<td>8</td>
<td>coal</td>
<td>LNG</td>
</tr>
<tr>
<td>9</td>
<td>deal</td>
<td>UK</td>
</tr>
<tr>
<td>10</td>
<td>Shell</td>
<td>rise</td>
</tr>
</tbody>
</table>

</div>

[[Paper with code](https://paperswithcode.com/paper/open-domain-event-extraction-and-embedding)] [[In Proceeding of CEUR Worshop](http://ceur-ws.org/Vol-2611/paper2.pdf)]

---
### Named Entity Recognition and Disambiguation (NERD) with Wikidata
This is my excuse to learn ReactJS, Docker, and deploying with EC2. I played around with online demos of NERD and found the performance a bit unexpected.

<div align="center">
  <figure>
  <img src="/assets/spacy_ner.gif"/>
     <figcaption>Short text queries are probably not spaCy main concern, for a good reason.  </figcaption>
     <figcaption>Accessed on 5th November 2020 </figcaption>
 </figure>
</div>

Is it possible to do NERD in short queries, where there are fewer grammar clues or capitalization like in a sentence? 
Would `watch [harry potter] vs read [harry potter]` be resolved to `Harry Potter film` and `Harry Potter book`?
I create a demo. I discovered that there are fewer datasets that deals with short query than I thought.

**Hardware:** 2 GBs RAM, 1 shared CPU

**What I like:** I devise tests to see if the cosine distances of different Word Embeddings suit the short text nature.

[[Demo](http://54.91.75.203/)][[Code](https://github.com/minhtriet/short_text_understanding)]
