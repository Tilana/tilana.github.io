---
layout: post
title: MediaUncovered
date: 2018-09-30 13:32:20 +0300
description: Uncover hidden bias in newspaper
img: media.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [NLP, media, Tools]
---


Free and diverse media is necessary for a well-informed public and a functioning society. However, objective reporting is not possible and sometimes newspapers even favor a certain ideology or political direction.

Even though we are not consciously aware of the presence of reporting biases, such as the tendency to favor arguments of a political party or to constantly set a country in a negative context, they do have  significant influence on our world view, our believes and on who we vote for.

The language newspapers use is a powerful tool to draw the attention of readers to a specific topic, to trigger emotions and to shape the public opinion. Do we talk about humans fleeing their country due to war or an invasion of migrants stealing our jobs and housing?

Knowing these biases helps to critically reflect the reliability and  trustworthiness of an article.



______



We build MediaUncovered, a free and open-source tool to uncover such hidden biases.

With statistical models it is possible to map millions and millions of newspaper articles into a vector space. In this vector space the relations and similarities of words are captures. This enables us to detect consistent reporting  biases, compare topic coverage and language usage of newspapers and even provide a basis to assess media variety in a country.

We want readers to explore the content and language of newspapers and critically reflect their sources of information. Journalist and media organizations can use the tool to detect and analyze underlying biases  in newspapers, investigate the language used when reporting about a  specific topic, find evidence for media consolidation and advocate for a free and diverse media landscape.

Watch [here](https://www.youtube.com/watch?v=2JgZPCWmseQ) our pitch for the AI grant.


## Method

First of all, we need to gather as many articles as possible from a newspaper source. Based on these articles we then use a statistical model to map each word into a vector space. These are so called word embeddings.
They allow us to analyse and compare the language of a newspaper.

The following links provide more information on word embeddings:

- [What the heck is Word Embedding](https://towardsdatascience.com/what-the-heck-is-word-embedding-b30f67f01c81)
- [Learning Word Embedding](https://lilianweng.github.io/lil-log/2017/10/15/learning-word-embedding.html)
- [Man is to Computer Programmer as Woman is to Homemaker? Debiasing Word Embeddings](https://arxiv.org/abs/1607.06520)
- [Rejecting the gender binary: a vector-space operation](http://bookworm.benschmidt.org/posts/2015-10-30-rejecting-the-gender-binary.html)



### Closely related words

Based on the word embeddings it is possible to determine which words are often used in the same context and are closely related.
For a media analysis this is helpful to understand the subtle language differences when talking about a specific topic. For example, when talking about migration often words like *flood or invasion of immigrations* are used. They have a negative connation and raise a sensation of helplessness and fear.

The word clouds below show two examples of words closely related to the keywords *flüchtling* (German: refugee - upper image) and *metoo* (lower image):

![]({{site.baseurl}}/assets/img/nn_fluchtling.png)

![]({{site.baseurl}}/assets/img/nn_metoo.png)



### Mapping Words

Mapping words means to align them on a axis. An axis determines the two extremes of a concept, such as good vs. bad, left-wing vs right-wing, male vs. female, etc.

When an axis is defined it is now possible to map certain keywords on this axis and compare them with others. For example, the first image below show a gender mapping in which the left side represents the female end of the axis and the right side the male extreme. The words on the y-axis are then mapped onto this gender axis and we can see that politics, physics, cars and aggressive are closer associated with men, while art, child, emotional are closer associated with female attributes.



![]({{site.baseurl}}/assets/img/mapping_gender.png)

![]({{site.baseurl}}/assets/img/mapping_politiker.png)



Word mapping make it possible to identify biases by visualizing the tendency of specific words being closer related to one extreme of a mapping axis.



### Analogies

Further, it is possible to create analogies with word embeddings.
An analogy explains the relationship of two objects by comparing them to a similar concept. For example:

 - *brother* is to *sister*, like *uncle* is to *aunt*
 -  *France* is to *Paris*, like *Germany* to *Berlin*



The following images show analogies for *seehofer* is to *merkel* like .... (upper image) and *conservative* is to *liberal* like ... (lower image).  



![]({{site.baseurl}}/assets/img/analogie_konservativ_liberal.png)

![]({{site.baseurl}}/assets/img/analogie_seehof_merkel.png)



 




## Contact us

Please find the full project code on [Github](https://github.com/MediaUncovered/Documents). 

Send us a message to [MediaUncoveredProject@gmail.com](https://github.com/MediaUncovered/Documents/blob/master/MediaUncoveredProject@gmail.com)


This project is funded by the PrototypeFund and the Federal Ministry of Education and Research.



|                 |                |
| :---------------------------------------: | :------------------------------------------------: |
| ![]({{site.baseurl}}/assets/img/bmbf.jpg) | ![]({{site.baseurl}}/assets/img/prototypefund.jpg) |