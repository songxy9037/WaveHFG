# [WaveHFG: High-Frequency Guidance for Heterogeneous Remote Sensing Image Change Detection with Wavelet Features](https://ieeexplore.ieee.org/document/11343859) (TGRS 2026)

[![Paper](https://img.shields.io/badge/Paper-IEEE_Xplore-blue)](https://ieeexplore.ieee.org/document/11343859)
[![Dataset](https://img.shields.io/badge/Dataset-GF--HCD-green)](#-gf-hcd-dataset)

---

### 📌 Quick Navigation
- [Abstract](#-abstract)
- [Core Methodology](#-core-methodology)
- [GF-HCD Dataset](#-gf-hcd-dataset)
- [Pretrained Weights](#-pretrained-weights)
- [Citation](#-citation)

---

## 📄 Abstract

Heterogeneous change detection (Hete-CD) between optical and synthetic aperture radar (SAR) images integrates detailed spectral information with all-weather observation capabilities. This approach aims to address the limitations of optical images, such as cloud cover and illumination variations, while mitigating speckle noise and enhancing the interpretability of SAR imagery. However, integrating these modalities poses challenges, including spectral inconsistencies and mismatched feature representations. To overcome these challenges, we propose a wavelet high-frequency guidance change detection (CD) network (WaveHFG). This approach utilizes wavelet-transform high-frequency features to enhance both the similarity and directional consistency of representations extracted from heterogeneous images. Our method incorporates two key modules: High-Frequency Differential-Guidance (Diff-G) and High-Frequency Directional-Guidance (Dir-G). These modules effectively capture subtle and often-overlooked details, hence improving the interpretability of the results. Additionally, the Frequency–Spatial Domain Difference Fusion (FSD$^2$F) module integrates features across multiple domains, providing a more comprehensive and detailed representation of change information. To rigorously evaluate the effectiveness of our proposed method, we constructed a new Hete-CD dataset with extensive coverage and increased complexity, encompassing a broader range of target categories to better reflect diverse real-world conditions. Extensive experiments on two publicly available datasets and our newly proposed dataset demonstrate that our method outperforms state-of-the-art CD methods.

---

## 🖼️ Core Methodology

### Network Architecture

![WaveHFG Structure](./figures/WaveHFG.png)  

*Figure: Construction of a heterogeneous remote sensing image CD network based on wavelet high-frequency guidance.*

---

## 📊 GF-HCD Dataset

We publicly release the **GF-HCD** dataset used in our paper for heterogeneous remote sensing image change detection.

### Download

| Item | Information |
|---|---|
| Dataset | `GF-HCD.zip` |
| Baidu Netdisk | [Download Link](https://pan.baidu.com/s/1906W9kTWUhENnhBjHC2Dzw?pwd=n5uq) |
| Extraction Code | `n5uq` |

### Dataset Structure

After downloading and extracting `GF-HCD.zip`, the dataset is organized as follows:

~~~text
GF-HCD/
├── A/
├── B/
├── label/
└── list/
~~~

**Where:**
- `A/` contains images from the first modality or time phase.
- `B/` contains corresponding images from the second modality or time phase.
- `label/` contains binary change masks.
- `list/` contains dataset split files.

### Usage Notice

The GF-HCD dataset is released for academic research purposes. If you use WaveHFG, the pretrained weights, or the GF-HCD dataset in your research, please cite our paper.

---

## 💾 Pretrained Weights

Pretrained weights for **WaveHFG** are available here:

- **Baidu Netdisk**: [Download Link](https://pan.baidu.com/s/1J64daf5cYQyb0leKoROOqQ)  
- **Extraction Code**: `ixus`

---

## 📜 Citation

If you find this work helpful for your research, please cite our paper:

~~~bibtex
@article{song2026wavehfg,
  title={WaveHFG: High-Frequency Guidance for Heterogeneous Remote Sensing Image Change Detection with Wavelet Features},
  author={Song, Xinyang and Gao, Yunhao and Zhang, Mengmeng and Li, Wei and Tao, Ran},
  journal={IEEE Transactions on Geoscience and Remote Sensing},
  year={2026},
  volume={64},
  number={},
  pages={1-14},
  publisher={IEEE}
}
~~~****
