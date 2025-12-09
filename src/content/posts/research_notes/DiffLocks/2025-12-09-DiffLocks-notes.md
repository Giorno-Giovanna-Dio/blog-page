---
title: Research Note -- DiffLocks - Generating 3D Hair from a Single Image using Diffusion Models.
published: 2025-12-09
pinned: false
description: Researhers - Radu Alexandru Rosu, Keyu Wu, Yao Feng, Youyi Zheng, Michael J. Black
tags: [科學, 論文]
category: 專題研究
draft: false
---

# Contributions of this paper:
1. Presented a 3D synthetic hair dataset consisting of 40K samples covering a wide variety of hairstyles.
    - They designed a large and very general geometry node network in Blender to generate various hairstyles.
2. Trained a novel diffusion framework called DiffLocks:
    - Used Hourglass Diffusion Transformers as a diffusion architecture.
    - Exploited features from a pretrained DINOv2 model.
        - DINOv2 features are richer than oreinted filters.
        ![DiffLocks Figure 6](./2025-12-09-DiffLocks-fig6.png)
3. Regressed the latent code for individual hair strands instead of guide strands, enabling the transformer to learn detailed spatial relationship between scalp and hair strand.
4. Modeled a desity map that defines the probability of a strand being generated at each location of the scalp.

# Figures
![DiffLocks Figure 1](./2025-12-09-DiffLocks-fig1.png)
![DiffLocks Figure 2](./2025-12-09-DiffLocks-fig2.png)
![DiffLocks Figure 3](./2025-12-09-DiffLocks-fig3.png)
![DiffLocks Figure 4](./2025-12-09-DiffLocks-fig4.png)
![DiffLocks Figure 5](./2025-12-09-DiffLocks-fig5.png)
![DiffLocks Figure 7](./2025-12-09-DiffLocks-fig7.png)
![DiffLocks Figure 8](./2025-12-09-DiffLocks-fig8.png)
