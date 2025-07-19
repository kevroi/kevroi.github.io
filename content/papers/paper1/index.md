---
title: "Goal-Space Planning with Subgoal Models" 
venue: "JMLR 2024"
date: 2024-10-22
lastmod: 2024-10-28
tags: ["Model-Based Reinforcement Learning","Temporal Abstraction","Planning"]
author: ["Chunlok Lo*","Kevin Roice*", "Parham Mohammad Panahi*", "Scott M. Jordan", "Adam White", "Gabor Michuz", "Farzane Aminmansour", "Martha White"]
description: "" 
summary: "We propose a long-horizon background-planning algorithm for online RL. This used subgoal
models (abstract in state & time) for faster long-term decision making & smarter value propagation." 
cover:
    image: "paper1.png"
    alt: "Abstract Models for Planning"
    relative: false
editPost:
    URL: "http://jmlr.org/papers/v25/24-0040.html"
    Text: "JMLR 2024"
downloads:
    - text: "Paper"
      url: "https://jmlr.org/papers/volume25/24-0040/24-0040.pdf"
    - text: "Poster"
      url: "paper1/GSP_Poster_ICML_v5.pdf"
    # - text: "Code"
    #   url: "https://github.com/your-repo/gsp"

---

---

##### Abstract

This paper investigates a new approach to model-based reinforcement learning using background planning: mixing (approximate) dynamic programming updates and model-free updates, similar to the Dyna architecture. Background planning with learned models is often worse than model-free alternatives, such as Double DQN, even though the former uses significantly more memory and computation. The fundamental problem is that learned models can be inaccurate and often generate invalid states, especially when iterated many steps. In this paper, we avoid this limitation by constraining background planning to a given set of (abstract) subgoals and learning only local, subgoal-conditioned models. This goal-space planning (GSP) approach is more computationally efficient, naturally incorporates temporal abstraction for faster long-horizon planning, and avoids learning the transition dynamics entirely. We show that our GSP algorithm can propagate value from an abstract space in a manner that helps a variety of base learners learn significantly faster in different domains.

---

##### Figure 6: Value Function update without (left) and with (right) Goal-Space Planning

![](paper1.png)

---

##### Download

+ [Paper](paper1.pdf)
+ [Poster](GSP_Poster_ICML_v4.pdf)
<!-- + [Code and data](https://github.com/pmichaillat/feru) -->

---

##### Citation

Lo C., Roice K., Panahi P.M., Jordan S.M., White A., Michuz G., Aminmansour F., White M. (2024) "Goal-Space Planning with Subgoal Models", *Journal of Machine Learning Research* Volume 25 (330) pages 1-57.

```BibTeX
@article{gsp2024,
author = {Chunlok Lo, Kevin Roice, Parham Mohammad Panahi, Scott M. Jordan, Adam White, Gabor Michuz, Farzane Aminmansour and Martha White},
year = {2024},
title ={Goal-Space Planning with Subgoal Models},
journal = {Journal of Machine Learning Research},
volume = {25},
number = {330},
pages = {1-57}}
```

---

<!-- ##### Related material

+ [Presentation slides](presentation1.pdf)
+ [Summary of the paper](https://www.penguinrandomhouse.com/books/110403/unusual-uses-for-olive-oil-by-alexander-mccall-smith/) -->
