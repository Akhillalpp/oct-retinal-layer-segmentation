# OCT Retinal Layer Segmentation

Deep learning–based retinal layer segmentation on Optical Coherence Tomography (OCT) images using advanced encoder–decoder architectures and composite loss engineering.

---

## 🧠 Overview

This project focuses on accurate multi-class retinal layer segmentation in OCT B-scan images.  
The objective is to improve boundary delineation and class-wise performance using architecture tuning and hybrid loss functions.

The work evaluates multiple architectures and compares them against state-of-the-art baselines across different OCT datasets.

---

## 🚀 Key Highlights

- Implemented and tuned **MultiResUNet** for OCT segmentation
- Designed a **composite loss function** combining:
  - Dice Loss
  - Cross-Entropy Loss
  - Focal Frequency Loss
  - Boundary Loss
- Evaluated performance using:
  - Dice Score
  - Pixel Accuracy
  - Balanced Accuracy
- Conducted cross-dataset evaluation on:
  - Duke OCT
  - HEG Dataset
  - Peripapillary OCT Dataset
- Compared against:
  - U-Net
  - Y-Net
  - GD-Net (state-of-the-art baseline)

---

## 🏗️ Model Architecture

The primary architecture used in this project is **MultiResUNet**, adapted and tuned for retinal OCT segmentation tasks.

Modifications include:
- Alpha scaling optimization for MultiRes blocks
- Custom composite loss integration
- Boundary-aware supervision

---

## 📊 Evaluation Metrics

| Metric | Purpose |
|--------|----------|
| Dice Score | Overlap measurement |
| Pixel Accuracy | Overall classification accuracy |
| Balanced Accuracy | Class imbalance handling |

---

## 🧪 Datasets

- Duke OCT Dataset
- HEG Dataset
- Peripapillary OCT Dataset

*(Datasets are not included due to licensing restrictions.)*

---

## 🛠️ Tech Stack

- Python
- PyTorch
- OpenCV
- NumPy
- Albumentations
- Matplotlib

---

## 📂 Project Structure

├── data/
├── models/
├── losses/
├── training/
├── evaluation/
├── configs/
└── main.py



---

## 🔍 Results

The tuned MultiResUNet model achieved competitive performance compared to state-of-the-art architectures, particularly improving boundary delineation and class-wise balanced accuracy.

Detailed quantitative results and visual comparisons are included in the `results/` directory.

---

## 🎯 Future Work

- Transformer-based segmentation models
- Self-supervised pretraining
- Real-time clinical deployment optimization
- Domain adaptation across OCT devices

---

## 🤝 Contributions

Open to collaboration in:
- Medical Image Segmentation
- Loss Function Engineering
- Clinical AI Applications

---

## 📫 Contact

Akhil Lal  
M.Tech Signal Processing  
LinkedIn: linkedin.com/in/akhillal

---

