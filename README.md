<div align="center">

<h1>SGLDet: Self-Guided Low Light Object Detection Framework</h1>

<p>
  <a href="https://openreview.net/forum?id=MGgAJ8yy2D">
    <img src="https://img.shields.io/badge/OpenReview-SGLDet-8c1b13?style=for-the-badge&logo=openreview" alt="OpenReview"/>
  </a>
  &nbsp;
  <a href="https://iclr.cc/virtual/2026/poster/XXXXX">
    <img src="https://img.shields.io/badge/ICLR-2026-4b44ce?style=for-the-badge&logo=openreview" alt="ICLR 2026"/>
  </a>
  &nbsp;
  <a href="https://gw-shin.github.io/sgldet-page/">
    <img src="https://img.shields.io/badge/Project%20Page-SGLDet-blue?style=for-the-badge&logo=githubpages" alt="Project Page"/>
  </a>
  &nbsp;
  <a href="https://github.com/gw-shin/SGLDet">
    <img src="https://img.shields.io/github/stars/gw-shin/SGLDet?style=for-the-badge&logo=github&color=yellow" alt="GitHub Stars"/>
  </a>
  &nbsp;
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/License-Apache%202.0-green?style=for-the-badge" alt="License"/>
  </a>
</p>

<!-- arxiv badge: uncomment when available
  <a href="https://arxiv.org/abs/XXXX.XXXXX">
    <img src="https://img.shields.io/badge/arXiv-XXXX.XXXXX-b31b1b?style=for-the-badge&logo=arxiv" alt="arXiv"/>
  </a>
-->

<!-- <p>
  <img src="https://img.shields.io/badge/DARK%20FACE-76.6%20mAP%20🏆%20SOTA-ff6f00?style=flat-square" alt="DARK FACE SOTA"/>
  &nbsp;
  <img src="https://img.shields.io/badge/ExDark-78.6%20mAP%20🏆%20SOTA-ff6f00?style=flat-square" alt="ExDark SOTA"/>
  &nbsp;
  <img src="https://img.shields.io/badge/nuImages%20Night-58.0%20mAP%20🏆%20SOTA-ff6f00?style=flat-square" alt="nuImages SOTA"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Inference%20Overhead-None%20✅-brightgreen?style=flat-square" alt="No Inference Overhead"/>
</p> -->

<br/>

 **[Self-Guided Low Light Object Detection Framework](https://openreview.net/forum?id=MGgAJ8yy2D)**  
> [Gwangik Shin](https://github.com/gw-shin) · Jaeha Song · Soonmin Hwang†  
> Department of Automotive Engineering, Hanyang University  
> ***ICLR 2026***

<br/>

<img src="assets/poster.jpg" alt="SGLDet Poster" width="100%"/>

</div>

---

## News

- [ ] Release pre-trained model weights
- [ ] HuggingFace / Gradio demo
- [x] `2026.01.22`: Paper accepted at **ICLR 2026** 🎉
- [ ] Code coming soon

---

## Overview

Object detection in low-light environments is inherently challenging due to **limited contrast and heavy noise**, both of which significantly degrade feature representations. We propose a novel **self-guided low-light object detection framework** that effectively addresses these issues **without introducing additional parameters or increasing inference time**.

Our method incorporates a **detachable auxiliary pipeline** used only during training, consisting of:
- An **Enhancing Module** (ε) — self-supervised low-light image enhancement
- A **Denoising Module** (D) — self-supervised noise suppression
- A **Fourier-domain Fusion Block** (F, F⁻¹) — structure-preserving target image construction

This pipeline is **completely removed at inference time**, incurring no additional computational cost over the baseline detector.

<p align="center">
  <img src="assets/overview.png" alt="SGLDet Overview" width="90%"/>
</p>

---

## Citation

If you find our work useful in your research, please consider citing our paper:

```bibtex
@inproceedings{shinself,
  title={Self-Guided Low Light Object Detection Framework},
  author={Shin, Gwangik and Song, Jaeha and Hwang, Soonmin},
  booktitle={The Fourteenth International Conference on Learning Representations}
}
```

---

## License

This software is released under the Apache 2.0 license. See [LICENSE](LICENSE) for details.

---

## Acknowledgement

This work was supported by the National Research Foundation of Korea (NRF) grant funded by the Korea government (MSIT) (No. RS-2024-00409492).
