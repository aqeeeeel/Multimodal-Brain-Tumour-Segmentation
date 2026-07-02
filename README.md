#  Text-Guided Brain Tumor Segmentation using Vision-Language Models

A multimodal deep learning framework for brain tumor segmentation that combines **FLAIR MRI images** with **radiology reports** using **Vision-Language Models**. The proposed architecture, **Swin-TextSegNet**, integrates image and text features to improve segmentation accuracy by leveraging semantic information from clinical reports.

---

##  Features

- Multimodal brain tumor segmentation using MRI images and radiology reports
- Swin Transformer-based visual encoder
- Frozen CLIP text encoder for extracting textual features
- Gated cross-attention module for image-text feature fusion
- Pixel-wise tumor mask prediction
- Trained and evaluated on the **BraTS 2020** dataset

---

##  Model Architecture

**Swin-TextSegNet**

- **Image Encoder:** Swin Transformer
- **Text Encoder:** Frozen CLIP Text Encoder
- **Fusion Module:** Gated Cross-Attention
- **Decoder:** Segmentation Decoder for pixel-wise mask prediction

The model aligns visual and textual representations to enhance tumor localization and boundary segmentation.

---

##  Results

| Metric | Score |
|---------|-------|
| Dice Score | **0.802** |
| IoU | **0.717** |
| Precision | **0.818** |
| Recall | **0.842** |

---

##  Tech Stack

- Python
- PyTorch
- MONAI
- Swin Transformer
- CLIP
- OpenCV
- NumPy
- Matplotlib

---

##  Dataset

**BraTS 2020**

The project uses FLAIR MRI scans and corresponding tumor segmentation masks from the BraTS 2020 dataset. Radiology reports are incorporated as textual input for multimodal learning.

---

##  Project Structure

```
Brain-Tumor-Segmentation/
│── notebook.ipynb
│── README.md
│── requirements.txt
│── images/
│── results/
```

---

##  Future Improvements

- Support multi-modal MRI sequences (T1, T1ce, T2, FLAIR)
- Fine-tune the CLIP text encoder
- Improve segmentation using larger Vision-Language Models
- Deploy the model as a web application for inference

---

