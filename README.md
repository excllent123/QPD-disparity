# All-directional Disparity Estimation for Real-world QPD Images

**CVPR 2025 Highlight Paper**

This is the official project page for our paper **"All-directional Disparity Estimation for Real-world QPD Images"**, accepted as a **Highlight paper** at *CVPR 2025*. In this work, we address the task of disparity estimation using Quad Photodiode (QPD) sensors, which are widely used in modern smartphone cameras. Our contributions include:

- 📷 The first large-scale real-world **QPD disparity dataset** (named **QPD2K**) with 2,100 high-resolution QPD image and ground-truth disparity pairs.
- 🔧 We propose the **DPNet** for DP disparity estimation and the **QuadNet** for QPD disparity estimation, with three novel modules fully considering the characteristics of QPD sensors. Our experiments demonstrate that our networks achieve SOTA performance in DP and QPD disparity estimation.

## 📁 Dataset: QPD2K

We introduce **QPD2K**, the first real-world dataset containing:
- 2,100 high-quality QPD raw images captured under diverse real-world scenarios.
- Corresponding disparity maps generated via calibrated stereo setups.

| Modality       | Count |
|----------------|-------|
| QPD Images     | 2,100 |
| Disparity Maps | 2,100 |

**Overview of QPD2K Generation Pipeline**
![QPD2K](https://github.com/excllent123/QPD-disparity/blob/main/figs/QPD2K_pipeline.jpg)

More details about the dataset can be found in the paper.

## 🔬 Method Overview

We propose two deep learning architectures:

- **DPNet Architecture Overview**
The DPNet comprises two novel modules: an illumination-invariant module and a coarse-to-fine module.
![DPNet](https://github.com/excllent123/QPD-disparity/blob/main/figs/Figure_network_DPNet.jpg)

- **QuadNet Architecture Overview**
QuadNet integrates two-directional information via an edge-aware fusion module for QPD data. A Census-based refinement further refines the fused disparity
![QuadNet](https://github.com/excllent123/QPD-disparity/blob/main/figs/Figure_network_Quad.jpg)

## 🧠 Code & Models

The QPD2K dataset, code and pre-trained models will be made publicly available soon after finalization. Please check back here for updates.

## 📄 BibTeX

If you find this dataset or method useful in your research, please cite our paper:

```bibtex
@inproceedings{yu2025qpd,
  author    = {Hongtao Yu  and Shaohui Song and Lihu Sun  and Wenkai  and Su Xiaodong Yang  and Chengming Liu},
  title     = {All-directional Disparity Estimation for Real-world QPD Images},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year      = {2025}
}
