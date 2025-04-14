---

# 🎓 Master Thesis: *Interpretation and Interpolation of Pixel Values - Improvement of Image Scaling Methods*

## 🗂️ Overview  
This repository contains the implementation and documentation of my Master's thesis titled **"Interpretation and Interpolation of Pixel Values - Improvement of Image Scaling Methods"**, submitted to Hochschule Wismar, Fakultät für Ingenieurwissenschaften, Bereich Elektrotechnik und Informatik. The thesis explores traditional and deep learning-based image super-resolution techniques, comparing their performance across various datasets.

## 🧠 Abstract  
The thesis presents an in-depth analysis of image scaling methodologies, focusing on pixel value interpretation and interpolation. It evaluates traditional techniques (Nearest Neighbor, Bilinear, Bicubic) and advanced deep learning approaches (SRCNN, ESPCN, Autoencoder, SRGAN) using metrics like PSNR, SSIM, and perceptual quality. The goal is to aid practitioners in selecting optimal techniques for applications in computer vision, image processing, and multimedia.

## ✨ Key Features  
- 🔁 **Traditional Methods**: Nearest Neighbor, Bilinear, and Bicubic interpolation.  
- 🤖 **Deep Learning Models**: SRCNN, ESPCN, Autoencoder, and SRGAN.  
- 📊 **Evaluation Metrics**: PSNR, SSIM, UQI, and processing time.  
- 🖼️ **Datasets**: Set5, Set14, Medical Images, and Satellite Images.
---
## ⚙️ Implementation Details  
### 🧩 Models  
1. **SRCNN**: A 3-layer CNN for super-resolution.  
2. **ESPCN**: Efficient sub-pixel convolutional network.  
3. **Autoencoder**: Uses subpixel and deconvolution upsampling.  
4. **SRGAN**: Generative adversarial network for perceptual quality enhancement.

### 📈 Training  
- **Dataset**: DIV2K (800 training, 200 validation images).  
- **Framework**: TensorFlow (implemented in Google Colab).  
- **Hyperparameters**: Learning rate, batch size, epochs, and loss functions (MSE).

### 🧪 Evaluation  
- **Metrics**: PSNR, SSIM, UQI, and processing time.  
- **Results**:  
  - ⚡ Autoencoder outperformed in metrics  
  - 🚀 SRCNN in speed  
  - 🎨 SRGAN in perceptual quality

---



## 🖼️ Sample Output

![Models_Output_Comparision](Interpretation-and-Interpolation-of-Pixel-Values-Improvement-of-Image-Scaling-Methods/Output
/Models_Output_Comparision.PNG)

---
## 📊 Results Summary  
| 🧠 Model        | 🔉 PSNR (dB) | 🧮 SSIM | 📐 UQI | ⏱️ Time (s) |
|----------------|--------------|--------|--------|------------|
| Autoencoder    | 31.36        | 0.71   | 0.96   | 1.32       |
| SRCNN          | 30.40        | 0.57   | 0.93   | <1e-5      |
| SRGAN          | 29.97        | 0.52   | 0.93   | 7.23       |

## 🔮 Future Work  
- 🧠 Extend training epochs and datasets  
- 📱 Develop web/mobile applications for upscaling  
- 🎥 Explore video super-resolution techniques  
- 🧾 Improve metric-based evaluations for GANs

## 📚 References  
See `thesis.pdf` for a full list of references.

## 🧾 Declaration  
The work is original, and all sources are properly cited. The electronic version matches the submitted thesis.

---

**👨‍💻 Author**: Mihir Pradip Patil  
**🎓 Supervisors**: Prof. Dr. Herbert Litschke, Prof. Dr.-Ing. Frank Krüger  
**📅 Submitted On**: 11.10.2023

---
