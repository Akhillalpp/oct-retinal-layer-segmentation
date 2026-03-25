# AN EFFICIENT LIGHTWEIGHT U-NET ARCHITECTURE FOR RETINAL LAYER SEGMENTATION IN OCT IMAGES

**Akhil Lal P.P., Deepthi V.R., Dr. Sudeep P.V., Dr. Sreelekha G.**  
National Institute of Technology Calicut  
📌 Presented as a Poster at AIML Systems Conference  

---

## 🧠 Introduction

- Retinal diseases such as Age-related Macular Degeneration (AMD), Diabetic Macular Edema (DME), among others, cause pathological changes in retinal layers, serving as biomarkers for diagnosis and monitoring.
- High-resolution OCT images enable retinal layer analysis, but manual evaluation is time-consuming, subjective, and impractical at scale.
- Deep learning models, including U-Net and its extensions, provide automated segmentation critical for accurate diagnosis.
- Portable and handheld OCT devices for point-of-care screening and teleophthalmology demand lightweight, efficient, and robust models that perform well across diverse imaging conditions.

---

## 💡 Our Contribution

In this work, we evaluate and enhance the performance of **MultiResUNet**, an extension of U-Net for automated segmentation of retinal layers and fluid regions in SD-OCT images using the Duke DME and Peripapillary datasets.

### Key Contributions:

- Extended MultiResUNet for the first time in retinal OCT layer segmentation with task-specific optimization.
- Tuned the filter scaling parameter (**α**) to enhance performance.
- Integrated a composite loss function combining region-based and contour-based terms.
- Performed comprehensive comparison with:
  - U-Net
  - Y-Net
  - LightReSeg
- Evaluated on:
  - Duke DME dataset
  - Peripapillary dataset

---

## ⚙️ Proposed Methodology

- Adopted MultiResUNet for retinal layer segmentation due to its effectiveness in:
  - Multi-scale feature extraction
  - Reduced semantic gap

### Architecture Highlights:

- **MultiRes Blocks**:
  - Capture multi-scale features
  - Use stacked 3×3 convolutions to approximate larger receptive fields
- **ResPaths**:
  - Reduce semantic gap between encoder and decoder
- **Scaling Parameter (α)**:
  - Controls number of filters
  - Tuned for optimal performance

---

## 🧪 Loss Function

The model uses a composite loss combining region and contour supervision:

### Total Loss: L_total = β1 * L_region + β2 * L_contour
