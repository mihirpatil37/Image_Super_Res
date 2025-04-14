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

## 📁 Repository Structure  
Got it! Here's your updated **Project Structure** section, formatted clearly with emojis and organized neatly to reflect the files and folders you mentioned:

---

## 📁 Project Structure

```
├── Autoencoder/
│   ├── Autoencoder_Subpixel_x2/
│   │   ├── Autoencoder_Subpixel_test_x2.ipynb
│   │   ├── autoencoder_subpixel_x2.ipynb
│   │   └── Autoencoder_subpixel_x2.h5
│   └── Autoencoder_Subpixel_x4/
├── Bicubic Interpolation/
│   └── Bicubic_Interpolation.ipynb
├── Bilinear Interpolation/
│   └── Bilinear_Interpolation.ipynb
├── ESPCN/
│   ├── ESPCNx2/
│   │   ├── ESPCN_test_x2.ipynb
│   │   ├── ESPCN_x2.ipynb
│   │   └── ESPCNx2.h5
│   ├── ESPCNx4/
│   │   ├── ESPCN_test_x4/
│   │   ├── ESPCN_x4/
│   │   └── ESPCNx4.h5
├── SRCNN/
│   ├── 2x/
│   │   ├── SRCNNx2.ipynb
│   │   ├── SRCNNx2_Test.ipynb
│   │   ├── srcnn_model_2x.h5
│   │   └── srcnn_model_2x_flickr8091.h5
│   ├── 4x/
│   │   ├── SRCNNx4.ipynb
│   │   ├── SRCNNx4_Test.ipynb
│   │   └── srcnn_4x.h5
├── SRGAN/
│   ├── srgan_test.ipynb
│   ├── srgan_train.ipynb
│   └── ckpt/
│       └── srgan_bicubic_x4/
├── Image_Data/
├── Results/
│   ├── output/
│   ├── accuracy.txt
│   ├── losses.txt
│   ├── training_and_validation_acc.png
│   ├── training_and_validation_loss.png
│   ├── SRRESNET_set5_x4_plot.png
│   ├── baby.png
│   ├── bird.png
│   ├── butterfly.png
│   ├── head.png
│   └── woman.png
├── TEST/
├── Model Evaluation & Plot/
│   └── Evaluation_and Plot/
├── Nearest Neighbour Interpolation/
│   └── NN_Interpolation.ipynb
├── PDFS/
│   ├── Master's Presentation.pptx
│   └── Master_Thesis.pdf
├── Figures/
│   ├── Autoencoder Deconvolution Parameters.png
│   ├── Autoencoder model structure.png
│   ├── Deep Neural Network.png
│   ├── Deep learning venn diagram.png
│   ├── ESPCN Parameters.png
│   ├── ESPCN model structure.png
│   ├── Interpolation image.png
│   ├── Literature Review.png
│   ├── SRCNN.png
│   ├── SRCNN_Parameters.png
│   ├── SRGAN_Parameters.png
│   ├── Set14.png
│   ├── Set14_coastgaurd.png
│   ├── Set5_Head.png
│   ├── Set5_Time.png
│   ├── Set5_results.png
│   ├── SharedScreenshot.png
│   ├── fig1.png
│   ├── fig2.png
│   ├── fig3.png
│   ├── fig5.png
│   ├── fig6.png
│   └── srcnn model structure.png
├── model_weights.h5
└── README.md

 
```

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

Below is a sample result from the SRGAN model tested on the Set5 dataset with 4× upscaling:

![SRRESNET_set5_x4_plot](Image_Super_Res/SRGAN/TEST/SRRESNET_set5_x4_plot.png)

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
