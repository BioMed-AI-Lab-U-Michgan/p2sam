# P<sup>2</sup>SAM
> Part-aware Prompted Segment Anything Model for Adaptive Segmentation\
> Chenhui Zhao and Liyue Shen\
> University of Michigan\
> [![arXiv](https://img.shields.io/badge/arXiv%20paper-2403.05433-b31b1b.svg)](https://arxiv.org/abs/2403.05433)&nbsp;

## Overview
<p align="center"><img src="/figures/github.jpg" style="width:96%; max-width:800px; height:auto;" class="center"></p>

We propose P<sup>2</sup>SAM, a training-free method that adapts a promptable segmentation model to new patients using only one-shot patient-specific data. 
P<sup>2</sup>SAM incorporates a **part-aware prompt mechanism** and a **distribution-based retrieval approach** to enhance generalization across:

- **Tasks:** P<sup>2</sup>SAM enhances generalization across different patient-specific segmentation tasks.
- **Models:** P<sup>2</sup>SAM can be plugged into various promptable segmentation models, such as SAM, fine-tuned SAM, and SAM 2.
- **Domains:** P<sup>2</sup>SAM performs effectively in both medical and natural image domains.

## Getting Started

Create an Python environment with:
```
conda env create -f environment.yaml
```

Prepare datasets with:
- [Datasets](data/README.md)

Prepare pre-trained and fine-tuned models with:
- [Models](pretrained_weights/README.md)

Fine-tune SAM on custom datasets (using SAM's iteratively training strategy) with:
- [Fine-tuning](fine_tuning/README.md)

Test P<sup>2</sup>SAM on out-of-distribution datasets with:
- [Testing](testing/README.md)

## Acknowledgement
This repository is built using the 
[DEiT](https://github.com/facebookresearch/deit/tree/main), 
[SAM](https://github.com/facebookresearch/segment-anything), 
[PerSAM](https://github.com/ZrrSkywalker/Personalize-SAM) 
repositories.

## Citation
If you find this repository helpful, please consider citing:
```bib
@article{zhaopart,
  title={Part-aware Prompted Segment Anything Model for Adaptive Segmentation},
  author={Zhao, Chenhui and Shen, Liyue},
  journal={Transactions on Machine Learning Research}
}
```