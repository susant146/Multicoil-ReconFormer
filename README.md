# 🌀 Multicoil ReconFormer for Accelerated MRI Reconstruction
This repository contains a customized implementation of ReconFormer—a transformer-based deep learning model for accelerated multicoil MRI reconstruction. We adapted the original ReconFormer architecture to support multicoil data by modifying the data loading and transformation modules from the original codebase.

> 🔴 **NOTE**: The code for multicoil fastMRI reconstruction will be available after the publication of our manuscript.

This repository provides a customized implementation of **ReconFormer** for **multicoil MRI reconstruction**, based on the original architecture proposed in the paper:

> **"ReconFormer: Accelerated MRI Reconstruction Using Recurrent Transformer,"** in IEEE Transactions on Medical Imaging, vol. 43, no. 1, pp. 582-593, Jan. 2024, doi: 10.1109/TMI.2023.3314747. 
> *P. Guo, Y. Mei, J. Zhou, S. Jiang and V. M. Patel*  
> [TMI:2023.3314747](https://ieeexplore.ieee.org/document/10251064)

We extend the original ReconFormer model to support **multicoil** reconstruction using the **fastMRI** dataset by adapting the dataloader and transformation modules.

---

## 📌 Highlights

- ✅ **Supports multicoil MRI data**
- ✅ Modified `SliceDataset` and `Transforms` for fastMRI multicoil knee dataset
- ✅ Consistent with fastMRI evaluation protocols (SSIM, PSNR, NMSE)
- ✅ Efficient training and inference pipelines
- ✅ Based on lightweight transformer design for fast and accurate reconstruction

---

## 📂 Requirements
torch>=1.11.0
torchvision>=0.12.0
h5py
numpy
matplotlib
tqdm
scikit-image
einops
pyyaml
fastmri @ git+https://github.com/facebookresearch/fastMRI.git

