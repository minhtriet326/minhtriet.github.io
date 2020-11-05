---
comments: false
excerpt: An overview and reflection of my portfolio
---
### Health hackathon
In 48 hours, my team created E-Prescription, an Android app to remind patients to take their medicine. 

**What I like:** In Vietnam, antibiotics are overused as one does not need doctor's prescription to buy some. This has caused Vietnam to be among the most overly tolerant antibiotic countries. This app is aim to solve this problem.

<div align="center" float="left">
<figure>
<img align="left" src="https://cdn.techinasia.com/wp-content/uploads/2013/11/jv-hacking-fest-vietnam-saigon-720x540.jpg" alt="drawing" width="350"/>
  <iframe width="350" height="263" src="https://www.youtube-nocookie.com/embed/2OjyYhaLu5w?start=9" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<figcaption>In the picture, I am the first from the right, top line. I am also the speaker in the video from 0:09 to 0:17</figcaption>
 </figure>
</div>

[[Our product is featured in Tech in Asia](https://www.techinasia.com/jv-hacking-fest-healthcare-hackathon-vietnam)][[Facebook page of the Hackathon, for more videos and photos](https://www.facebook.com/jvhackingfest/?fref=nf)] 


### Bachelor thesis
Use Machine Learning to fix [shibboleth for Vietnamese language speakers](https://en.wikipedia.org/wiki/Vietnamese_phonology#Initial_consonants)

**What I like:** Big impact, as 22.27% teachers and students of the capital city ([Source in Vietnamese](https://kenhtuyensinh.vn/gan-47000-giao-vien-va-hoc-sinh-noi-ngong)) suffers from shibboleth. I lead the team, and this project introduced me to machine learning and tried my hand at data collection and model deployment.

### Industrial robotics software
Pose estimation on a table top environment, with whole dataset consist of two images. My work is in University of Bonn's work in EuroC Challenge.


[EuroC Challenge](https://web.archive.org/web/20191204203324/http://www.euroc-project.eu/index.php?id=nimbro_manufacturing), [Paper](\href{https://arxiv.org/abs/2001.04134)

**What I like:** How I adapted when the training data consists of RGBD data of one images, and still deliver (Citroën bought our work!)

### Rapid road detection
Road detection with 50% faster intepretation time and retain more than 95% quality. 

<p align="center">
  <figure>
  <img src="/assets/segmented.gif"/>
     <figcaption>Green means another lane or intersected road, pink is the road the car currently on</figcaption>
 </figure>
</p>

**What I like:** My first computer vision project. Seeing the result of the work in the visual form was quite a sensation.

[Implementation](https://github.com/minhtriet/clockwork-kitti) [Paper](https://arxiv.org/pdf/2010.15250.pdf)

### Master thesis
Gas price prediction

**What I like:** I step away from accepting the model as the black box and try to wrestle some sense out of it, which I found most papers that I've read lagging behind. Top ten most influential words to gas price according to my model. It is the table 6 in my work.

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

### Named Entity Recognition and Disambiguation (NERD) with Wikidata
My excuse to learn ReactJS, Docker and deploying with EC2. I also played around with online demos of NERD and find the performance a bit unexpected.

<div align="center">
  
  <figure>
  <img src="/assets/spacy_ner.gif"/>
     <figcaption>Short text queries are probably not spaCy main concern, for a good reason. Accessed on 5th November 2020 </figcaption>
 </figure>
 
</div>

Is it possible to do NERD in short queries, where there is fewer grammar clues or captitalization like in a sentence? 
Would `watch [harry potter] vs read [harry potter]` be resolved to `Harry Potter film` and `Harry Potter book`?
I create a demo . I discovered that there are fewer dataset that deal with short text than I thought. Twitter datasets are an option, but developer has to deal with @ mention while I envisioned this as more of a search machine.

**What I like:** I divise tests to see if cosine distance of different Word Embeddings suit the short text nature.

[Demo](http://54.91.75.203/)
