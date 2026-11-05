# INVAR

## Randomization-Invariant Visual Representations for Zero-Shot Sim-to-Real

**Sunshine Jiang, Shuo Cheng, Francois Robert Hogan, Matthew Chang, Tingfan Wu, Jitendra Malik, Karen Liu, Nur Muhammad Mahi Shafiullah, Akash Sharma**

[Project website](https://xinyunsunshine.github.io/INVAR/)

INVAR learns visual invariance from paired clean and randomized simulation renders. The pretrained encoder is frozen and reused across downstream policies trained on clean simulation images, enabling zero-shot transfer to real robots.

The website presents the method, real-world robot demonstrations, attention and feature visualizations, scaling experiments, and general-vision trade-offs. This repository contains the **website and media**; training code and model checkpoints are not included in this website release.

## View locally

No build step or package installation is required:

```sh
git clone https://github.com/xinyunsunshine/INVAR.git
cd INVAR
python3 -m http.server 8765
```

Open [localhost:8765](http://localhost:8765).

## Website source

- `index.html`: project narrative, authors, figures, and resource links.
- `style.css`: responsive layout and visual styling.
- `script.js`: video controls, example selectors, state-matched renders, and results charts.
- `assets/`: project figures, video clips, poster images, and visualization metadata.

Videos include playback controls and respect reduced-motion preferences. Quantitative results distinguish the main benchmark from the separate scaling and ablation evaluations. Feature-PCA colors represent principal components, not semantic classes.

## Deployment

GitHub Pages serves the root of `main` at [xinyunsunshine.github.io/INVAR](https://xinyunsunshine.github.io/INVAR/). Pushing website changes to `main` triggers deployment. `.nojekyll` enables direct static hosting, and relative asset paths support the `/INVAR/` project URL.

## Acknowledgments

The website design draws inspiration from [EigenDEXplore](https://eigendexplore.github.io/). The Sharpa hand reference image is from [its hand gallery](https://eigendexplore.github.io/assets/s5/hands/sharpa.webp).
