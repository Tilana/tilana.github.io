---
layout: post
title: Capturing political and ideological biases with word embeddings
date: 2017-01-07 13:32:20 +0300
description: Graph-based semi supervised learning for text classification
img: bias_russia_us.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [NLP, media]
---



Newspapers provide us with information about the world and have significant influence on our opinions, as well as our behaviour. Despite the journalistic principle of objectivity, the extent at which certain topics are covered in media, as well as the opinions expressed about political situations depend heavily on the newspaper and the country it is published in.

In this project we will investigate whether political biases in news articles can be captured with word embeddings. Training a neural network on a large corpus of text documents creates a vector space that is able to preserve semantic relations between words. These so called *word2vec* models dependent on the word context that is provided by the text documents they are trained on. Therefore, consistent political and ideological bias in newspapers should affect the relations in the *word2vec* model such that compared with a different model these biases can be identified.

Based on the assumption that media in the US and Russia express diverging opinions regarding certain political issues, two models trained on these databases will be analyzed and compared regarding their view on their own and the opposing state.



<embed src="{{site.baseurl}}/assets/pdf/PoliticalBiasesWord2Vec.pdf" width=1000 height=1200 type="application/pdf">


______







This project paper was written for a text mining course during my Master program at Radboud University.

It is the foundation of [MediaUncovered](https://github.com/MediaUncovered), a project to uncover hidden bias in media with word embeddings. 