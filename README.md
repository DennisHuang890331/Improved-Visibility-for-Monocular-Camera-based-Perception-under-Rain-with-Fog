# Improved Visibility for Monocular Camera-based Perception under Rain with Fog
### An Efficient Vision Transformer Approach with Depth-Guided Spatial Feature Transform (DG-SFT) and Semantic Loss

[![Paper](https://img.shields.io/badge/Paper-ScienceDirect-red)](https://www.sciencedirect.com/science/article/pii/S0957417425042769)
[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.eswa.2025.130661-blue)](https://doi.org/10.1016/j.eswa.2025.130661)
[![TF](https://img.shields.io/badge/TensorFlow-%3E%3D2.10-orange)](#installation)

Official Keras implementation of the ESWA paper:
**“Improved Visibility for Monocular Camera-based Perception in Autonomous Driving Systems under Rain with Fog: An Efficient Vision Transformer Approach.”**

## Abstract
Adverse weather degrades image quality and undermines the reliability of monocular camera-based perception in autonomous driving. Most existing deraining methods primarily remove rain streaks while overlooking fog-like effects, which further obscure distant scene details and harm downstream perception. This work presents an efficient Vision Transformer (ViT)-based restoration framework that addresses both rain streaks and fog without compromising perception accuracy. The proposed model introduces a Depth-Guided Spatial Feature Transform (DG-SFT) block that leverages depth information predicted by a lightweight CNN decoder and is designed based on a mathematical rain model to mitigate distance-dependent haze. In addition, we propose a semantic loss that constrains the discrepancy between segmentation outputs of the original and restored images. Experiments on RainCityscapes and real-world rainy images show improved PSNR/SSIM over prior ViT- and CNN-based baselines, while achieving 7.86 ms inference latency, supporting latency-critical deployment.

## Model Architecture

<p align="center">
  <img src="image/README/Architecture.png" width="95%">
</p>
<p align="center"><em>Overview of the proposed network.</em></p>

## Comparison on RainCityscapes
<p align="center">
  <img src="image/README/1732081399839.png" width="95%">
</p>
<p align="center">
  <img src="image\README\2026-02-23 144923.png" width="80%">
</p>


## Analysis on downstream task
<p align="center">
  <img src="image\README\1732081441406.png" width="95%">
</p>
<p align="center">
  <img src="image\README\1231256876867.png" width="95%">
</p>
