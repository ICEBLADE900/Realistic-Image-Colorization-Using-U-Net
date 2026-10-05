# 🎨 Realistic Image Colorization Using U-Net

A deep learning project that automatically converts **black-and-white (grayscale) images into color images** using a **U-Net-based image-to-image translation model**.

## 📌 Project Overview

Image colorization is the process of adding realistic colors to grayscale or black-and-white images. Since grayscale images do not contain the original color information, predicting appropriate colors is a challenging computer vision problem.

This project develops a **U-Net deep learning model** that learns the mapping between grayscale images and their corresponding RGB color images. The model uses an **encoder-decoder architecture with skip connections** to preserve important image details such as edges, shapes, textures, and object boundaries.

## 🚀 Key Features

* 🖼️ Automatic grayscale-to-color image conversion
* 🧠 U-Net based deep learning architecture
* 🔄 Encoder-decoder structure with skip connections
* 🎯 Supervised image-to-image translation
* 📉 L1 reconstruction loss for training
* ⚡ Adam optimizer
* 📊 Image-quality evaluation using MSE, PSNR, and SSIM
* 👁️ Visual comparison of input, original, and colorized images
* 💻 Implemented using Python and PyTorch
* ☁️ Can be trained using Google Colab and GPU acceleration

## 🔄 Workflow

```text
Color Image
     ↓
Grayscale Conversion
     ↓
Image Preprocessing
     ↓
U-Net Model
     ↓
Predicted RGB Image
     ↓
Loss Calculation
     ↓
Model Training
     ↓
MSE / PSNR / SSIM Evaluation
```

## 🏗️ Model Architecture

The U-Net consists of:

* **Encoder** – extracts image features such as edges, shapes and textures.
* **Bottleneck** – learns high-level representations.
* **Decoder** – reconstructs the color image.
* **Skip Connections** – transfer spatial information from the encoder to the decoder, helping preserve fine details.

The basic feature progression in the encoder is:

```text
1 → 64 → 128 → 256 → 512
```

## 🛠️ Technologies Used

* Python
* PyTorch
* NumPy
* OpenCV / PIL
* Matplotlib
* Google Colab
* Deep Learning
* Convolutional Neural Networks
* U-Net

## 📊 Evaluation

The trained model is evaluated using:

| Metric | Purpose                         |
| ------ | ------------------------------- |
| MSE    | Measures pixel-level error      |
| PSNR   | Measures reconstruction quality |
| SSIM   | Measures structural similarity  |

Visual comparison is also performed between the **grayscale input, original RGB image, and predicted colorized image**.

## 🎯 Applications

* Restoration of historical photographs
* Automatic photo enhancement
* Digital media processing
* Computer vision
* Image-to-image translation
* AI-assisted image restoration

## ⚠️ Limitations

Colorization is inherently ambiguous because a grayscale image can correspond to multiple possible color versions. Performance can also depend on the size and diversity of the training dataset, while complex scenes and unusual objects may produce inaccurate colors.

## 🔮 Future Improvements

Future versions can improve realism by using:

* Perceptual loss
* GAN-based colorization
* Attention mechanisms
* Larger and more diverse datasets
* User-controlled color guidance
* More advanced perceptual evaluation metrics

## 👨‍💻 Authors

**Arpit Raj**
Department of Electronics and Communication Engineering
Bharati Vidyapeeth (Deemed to be University) College of Engineering, Pune

**Shatakshi Sinha**
Department of Electronics and Communication Engineering
Bharati Vidyapeeth (Deemed to be University) College of Engineering, Pune

## 📚 References

1. Ronneberger et al., *U-Net: Convolutional Networks for Biomedical Image Segmentation*, MICCAI 2015.
2. Larsson et al., *Learning Representations for Automatic Colorization*, ECCV 2016.
3. Zhang et al., *Colorful Image Colorization*, ECCV 2016.
4. Iizuka et al., *Let there be Color!*, ACM Transactions on Graphics, 2016.
5. Isola et al., *Image-to-Image Translation with Conditional Adversarial Networks*, CVPR 2017.
