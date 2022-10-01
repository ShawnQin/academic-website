---
title: Optimal nonlinear compressed sensing in olfactory periphery
summary: To achieve efficient coding of odor information in an array of nonlinear olfactory receptors, the odor-receptor sensitivity matrix must be sparse. This sparsity depends on the statistics of environmental odors. We used analytical calclation and extensive numerical simulation to study the optimal sensitivity matrix for recptors with and without spontaneous (background) activity.
tags:
  - olfaction
date: '2022-10-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  placement: 2
  caption:
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
The periphery sensory systems are the gateway between the physical world and the brain. Olfaction plays a vital role in the survival of many animals. A fundamental question in olfaction is how to represent and process the environmental odors, which are typically mixtures of a few odorants from a huge number of possible odorants, each with a broad distribution of concentrations. While the possible odorants and their mixture in the natural environment is much larger than the number of olfactory receptor neurons (ORNs), which respond to odorant concentration non- linearly (sigmoidal) with a finite sensitivity range. Thus, how to encode numerous sparse odor mixtures with a relatively small number of nonlinear ORNs – the nonlinear compressed sensing problem – remains a puzzle.

Using an information theory approach, I studied the optimal coding strategies that enable nonlinear ORNs to best represent olfactory information (both the odorants’ identities and their concentrations) in sparse odor mixtures. I showed that the optimal odor-receptor sensitivity matrix is sparse, and the nonzero sensitivities follow a broad distribution (matching the statistics of the odorants), both of which are consistent with existing experiments. For ORNs with a finite basal activity, my study shows that co-existence of both odor-evoked excitation and inhibition increases coding capacity, which provides a plausible explanation for such co-existence observed in the fly olfactory system. Furthermore, I showed that coding the inputs with the optimal sensitivity matrix can enhance the accuracy of the downstream decoding and learning tasks. These general statistical properties of the optimal sensitivity matrix for nonlinear compressed sensing may shed light on understanding the peripheral olfactory sensory system.
