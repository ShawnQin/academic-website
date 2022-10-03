---
title: Biologically plausible supervised learning algorithm
summary: Biologically plausible networks models with noisy synaptic update explain the widely observed representational drift.
tags:
  - biolgically plausible learning
date: '2022-10-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Summary of the contrastitive similarity matching
  focal_point: Smart

links: ''
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/ShanshanQin_/status/1433828229098311680
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---

Learning in the brain requires the change of synaptic strength across a large population of neurons. How does the brain modify and coordinate individual synapses in the face of limited information available to each synapse in order to achieve a global learning task, the credit assignment problem, has puzzled scientists for decades. While artificial neural networks (ANNs) have achieved supra-human performance in many tasks, training such networks relies on algorithms such as error back-propagation algorithm, which is unlikely implemented in the brain. To understand how the brain solve the credit assignment problem at the algorithm level, any biologically plausible learning rules must respect the biological constraints. For example, learning in natural networks must operate in the online (streaming) setting, rather than offline (batch) setting. That means the network takes input sequentially and the output is generated before new input is taken. Another key constraint is that biologically plausible learning algorithm must be local, only depends on the activity of presynaptic and postsynaptic neurons.

Based on previous works on biologically plausible unsupervised learning, we proposed a novel biologically plausible supervised learning algorithm derived from an objective function motivated by the following observations: 1) the object representations along the ventral visual pathways of the brain and deep neural networks, where representations of objects belong to the same category gradually becomes similar, while objects of different categories become less similar. This suggests a layer-wise learning goal in a deep network: each layer aims to learn a representational similarity matrix that interpolates between previous and later layers. 2) error signal during learning can be extracted from the change of stationary neural activities when operating in two different modes, free and clamped phase. Therefore, a learning rule can be derived from a contrastive function which is the difference of cost function between the two phases. Combing these two facts, I formulated a contrastive similarity matching objective function and derive from it deep neural networks with feedforward, lateral, and feedback connections and neurons that exhibit biologically plausible Hebbian and anti-Hebbian plasticity.

> S. Qin, N. Mudur, C. Pehlevan,“[Contrastive Similarity Matching for Supervised Learning](https://direct.mit.edu/neco/article-abstract/33/5/1300/97484/Contrastive-Similarity-Matching-for-Supervised?redirectedFrom=fulltext)”, Neural Computation 33(5), 1300 (2021).