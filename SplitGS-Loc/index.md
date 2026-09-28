---
layout: project
title: Disambiguating 2D-3D Correspondences in Gaussian Splatting-based Feature Fields for Visual Localization
keywords: Visual Localization, Gaussian Splatting, Feature Fields
authors:
    - {name: "Miso Lee", link: "https://misoleekr.github.io/", org: 0}
    - {name: "Sangeek Hyun", link: "https://hse1032.github.io/", org: 1}
    - {name: "Yerim Jeon", link: "https://jyerim.github.io", org: 0}
    - {name: "Jae-Pil Heo", link: "https://sites.google.com/site/jaepilheo", org: 0, corresponding: "True"}
affiliations:
    - "Sungkyunkwan University"
    - "NAVER LABS"

paper_link:
supplementary_link:
arxiv_link: https://arxiv.org/abs/2605.07351
github_link: https://github.com/misoleekr/SplitGS-Loc
openreview_link:
conference: NeurIPS 2026

tldr: SplitGS-Loc exploits Gaussian attributes for localization, stabilizing the Perspective-n-Point algorithm and achieving strong localization accuracy and mapping efficiency.

data_host: &data_host "/SplitGS-Loc/resources"

title_image:
    url: /SplitGS-Loc/resources/title_image.jpg

sections:
    - title: "Abstract"
      is_light: is-light
      paragraphs:
        - type: text
          content: >-
            While Gaussian Splatting-based Feature Fields (GSFFs) have shown promise for visual localization, this paper highlights that photometrically optimized GSFFs are inherently ill-suited for 2D-3D matching. The volumetric extent of each Gaussian induces many-to-one pixel-to-point mappings that destabilize PnP-based pose estimation, while photometric optimization gives rise to superfluous Gaussians devoid of multi-view consistency. To address these issues, we propose SplitGS-Loc, a localization-specialized GSFFs construction framework that disambiguates 2D-3D correspondences by exploiting Gaussian attributes. Our key design, Mixture-of-Gaussians-based splitting, decomposes each Gaussian into smaller Gaussians, replacing ambiguous many-to-one with precise one-to-one correspondences. In parallel, we exploit composition weights from GS rasterization to select Gaussians that significantly and consistently contribute across multiple views and aggregate discriminative features through strong pixel-Gaussian associations, enforcing multi-view consistency. The resulting compact yet discriminative feature fields enable stable PnP convergence, achieving state-of-the-art performance on localization benchmarks. Extensive experiments validate that SplitGS-Loc extends the utility of photometric GSFFs to accurate and efficient localization by exploiting Gaussian attributes, without per-scene training or iterative pose refinement.
  
bibtex: >-
  @article{lee2026splitgsloc,
    title={Disambiguating 2D-3D Correspondences in Gaussian Splatting-based Feature Fields for Visual Localization},
    author={Lee, Miso and Hyun, Sangeek and Jeon, Yerim and Heo, Jae-Pil},
    journal={arXiv preprint arXiv:2605.07351},
    year={2026}
  }
---
