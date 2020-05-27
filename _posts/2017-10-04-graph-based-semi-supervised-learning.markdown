---
layout: post
title: Graph-based Semi-supervised Learning for Text Classification
date: 2017-10-04 13:32:20 +0300
description: Graph-based semi supervised learning for text classification
img: graph_based_classification.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [NLP, Text Classification]
---



In this paper, we propose a graph-based representation of document collections in which both documents and features are represented by nodes. The nodes are connected with weights based on word order, context similarity and word frequency. Graph-based representations can overcome the limitations of bag-of-words based representations that suffer from sparseness for collections with short documents. In a series of experiments, we evaluate multiple types of graph-based text features in the context of semi-supervised text classification, and investigate the effect of the number of labeled documents in the collection. We find that graph-based semi-supervised learning outperforms bag-of-words semi-supervised learning but not bag-of-words supervised learning in 20-class text categorization. A large asset of graph-based representations is that they are flexible in the types of nodes and relations that are included.





______







This paper is a result of my Master thesis. It was published in October 2017 at the *ICTIR: Proceedings of the ACM SIGIR International Conference on Theory of Information Retrieval* in Amsterdam.

Access the full [paper](https://dl.acm.org/doi/10.1145/3121050.3121055) on the ICTIR website or directly open the [pdf](https://dl.acm.org/doi/pdf/10.1145/3121050.3121055).