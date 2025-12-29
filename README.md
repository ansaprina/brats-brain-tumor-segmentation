# Multiclass Brain Tumor Segmentation on BraTS 2021 Dataset

This repository explores multiclass segmentation of brain gliomas using the MICCAI BraTS 2021 challenge dataset. It includes Jupyter notebooks for exploratory data analysis (EDA), model training, and inference/visualization.

### Models implemented and compared:

 - U-Net (2D)
 - nnU-Net v2 (2D and 3D configurations)
 - MedNeXt (3D)

The BraTS 2021 dataset provides multi-modal MRI scans (T1, T1CE, T2, FLAIR) with expert annotations for three tumor sub-regions:

 - NCR/NET — Necrotic and non-enhancing tumor core (label 1)
 - ED — Peritumoral edema (label 2)
 - ET — GD-enhancing tumor (label 4)

Hierarchical metrics evaluate whole tumor (WT), tumor core (TC), and enhancing tumor (ET).

### Repository Contents
```
brats-brain-tumor-segmentation/
├── .gitattributes
├── .gitignore
└── notebooks/
    ├── 01_EDA.ipynb  → Dataset statistics and visualization
    ├── 02_unet_baseline.ipynb → Custom U-Net implementation
    ├── 02_unet_baseline_full.ipynb → Custom U-Net implementation
    ├── 02_unet_inference.ipynb → Custom U-Net implementation
    ├── 03_nnunetv2_2D.ipynb → nnU-Net 2D setup and training
    ├── 03_nnunetv2_2D_inference.ipynb → nnU-Net 2D inference
    ├── 04_nnunetv2_3D.ipynb → nnU-Net 2D setup and training
    ├── 04_nnunetv2_3D_inference.ipynb → nnU-Net 3D inference
    └── 05_MedNeXt_M_5.ipynb → MedNeXt M 5 3D setup, training and inference
```
