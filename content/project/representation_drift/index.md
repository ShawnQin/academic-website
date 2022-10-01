---
title: Representational drift
summary: Biologically plausible networks models with noisy synaptic update explain the widely observed representational drift.
tags:
  - drift
date: '2022-10-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Summary of the representational drift
  focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ShanshanQin_/status/1433828229098311680
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

The brain forms association between external stimuli with internal neural population activities during memory acquisition. This population neural activities during memory recall are termed “neural representations”. Conventionally, stable memories and stereotyped behaviors are thought to be associated with stable neuronal representations. However, recent experiments with longitudinal recording in free- behaving animals have showed that neuronal activities in cortical areas that are essential for specific tasks undergo continuous reorganization even after the animals have fully learned their tasks, a phenomenon termed “representational drift”. The prevalence of such drift naturally leads to questions about is origin, dynamics, and implementations.

Motivated by the observation that synapses in the brain are highly dynamic even in the absence of neural activity, I hypothesized that representational drift can be accounted by a learning process with noisy synaptic dynamics and a degeneracy of possible learned representations. We focused on representational drift in brain areas where neurons have localized receptive field (RFs), such as hippocampal place cells. In these systems, population of neurons with “bump” RFs tile the parameter space they encode. We tested this hypothesis using a minimum biologically plausible network: the Hebbian/anti-Hebbian network endowed with noisy synaptic update. These networks are ideal model because they optimize similarity-based representational objectives with degenerate optima. Via both theoretical calculation and numeric simulations, I showed that drift of individual RFs can be characterized by a coordinated random walk, with the diffusion constants depending on various parameters such as learning rate, noise amplitude, and input statistics. This model not only recapitulates experimental observation in hippocampus and posterior parietal cortex, but also make several interesting predictions: 1) Neurons whose synapses have faster turnover dynamics exhibit faster drift, 2) RF with large peak firing rate tend to be more stable, 3) Contribution of different source of synaptic noise, for example, forward synaptic noise has larger effect on RF drift compared with that of collateral synapse, 4) the drift of RFs are coordinated in a specific way to preserve the representational similarity.