# IIRS_ISRO_Internship_Project
This project, developed during my IIRS ISRO internship, uses a custom ResNet50 model for building identification in Delhi NCR from Sentinel-2 satellite imagery. It addresses challenges like low resolution and data quality, contributing to urban planning and sustainable development through automated urban infrastructure detection.

---

# Building Segmentation from Satellite Imagery using ResNet50

## 🎯 Objective

To develop a custom deep learning-based image segmentation model using a ResNet50 encoder and U-Net decoder for identifying buildings in Sentinel-2 satellite imagery of the Delhi NCR region. The goal is to assist urban planning efforts by generating accurate building masks.

## 🗂️ Dataset Used

* Sentinel-2 satellite imagery (2023) focused on Delhi NCR
* Images tiled into 256×256 pixels
* Masks annotated for building regions
* Resolution enhanced via 4x Super Resolution (ESRGAN)

## 👩‍💻 Contribution

* Designed and trained a hybrid ResNet50 + U-Net segmentation model
* Preprocessed and normalized imagery and masks
* Applied super-resolution to improve input quality
* Performed evaluation using metrics like IoU, accuracy, and Dice coefficient
* Attempted generalization on different city zones

## ✅ What Worked

* Model successfully segmented building regions with reasonable accuracy
* Custom preprocessing pipeline with normalization and super-resolution improved inputs
* Training loop and evaluation setup worked without major issues

## ❌ What Didn’t

* **Low-resolution data** led to distorted predictions despite super-resolution
* Building edges often tore apart due to pixel tearing in low-detail regions
* Class imbalance and unclear mask boundaries affected performance in complex urban scenes
* not good iu score and dice coefficient

## 🔧 Future Improvements

* Collect higher-resolution, cleaner satellite data
* Add attention mechanisms or transformers to refine edge detection
* Fine-tune with more balanced datasets
* Test model on rural vs. urban variations and multi-class segmentation

---
