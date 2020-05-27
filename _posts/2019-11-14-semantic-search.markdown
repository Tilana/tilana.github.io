---
layout: post
title: semantic search
date: 2019-11-14 00:00:00 +0300
description: Semantic Search - Find what you are looking for
img: semantic_search.jpg # Add image post (optional)
tags: [NLP, Tools] # add tag
---



With huge amounts of information being accessible, effectively browsing through this information is crucial.  Search is powerful. However, most of the time it is limited to the keywords which we feed into a search engine. Small spelling mistakes can screw up the search or if looking for a wide topic, searching for each keyword of an association map quickly turns into a tedious and messy process.
Also, in unfamiliar expert domains, we might not even know the search terms that yield the results which we expect.



Semantic search is a tool to search not only for a specific keyword, but also for associated words and similar concepts.

For example whehttps://fasttext.cc/docs/en/unsupervised-tutorial.htmln searching for *hate speech* phrases with similar concepts, such as *offensive, inflammatory speech, insulting terms, defamation, etc.* appear in the search results.


The demo below show the integration of semantic search into [Uwazi](https://github.com/huridocs/uwazi/):

<iframe src="{{ site.baseurl }}/assets/img/semantic_search.mp4" 
    width="900" 
    height="500"
    frameborder="0" 
    allowfullscreen>
</iframe>


It is possible to determine the exploration ratio. The smaller, the closer the search results match the actual search term. Also, it is possible to set a minimum number of sentences in a document that have to include the search concept in order for it to show up in the results.
For each sentence with the search term a confidence score is displayed.

____________



While Uwazi provides a UI for semantic search, it is also possible to use the tool in the terminal.

For the code and setup instructions see the [Github repository](https://github.com/Tilana/semantic-search). 



### Model

The semantic search tool is built upon a *fasttext* word embedding. With a sliding window the cosine distance of the averaged embeddings of the search term and a sentence in a document are compared. If this similarity exceeds a threshold, the sentence is shown in the search results.

With fasttext it is easy to adapt the word embeddings to a specific domain, e.g. legal documents on human rights, which will significantly improve the results.

Please note that, due to storage limitations, the model stored in the repository is a dummy model which does not yield reliable search results.

For information on how to train a fasttext model have a look at their documentation on [word representations](https://fasttext.cc/docs/en/unsupervised-tutorial.html).