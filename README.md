# Anime Faces Generation with DCGAN

<p align="center">
  <img src="outputs/Screenshot 2025-09-09 183853.png" alt="Sample Anime Faces" width="400"/>
</p>

**Description:**  
This project implements a <b>Deep Convolutional Generative Adversarial Network (DCGAN)</b> to generate realistic anime face images. Built with <b>TensorFlow</b> and <b>Keras</b>, it demonstrates how GANs learn to produce images from random noise vectors.

## Project Overview

- <b>Generator:</b> Converts random noise vectors into 64×64 RGB anime face images using Dense, Conv2DTranspose, and ReLU layers.  
- <b>Discriminator:</b> Distinguishes real vs. generated images using Conv2D, MaxPooling2D, and LeakyReLU layers.  
- <b>DCGAN Class:</b> Combines Generator and Discriminator with custom training steps.  
- <b>Visualization:</b> Generates and displays sample images at the end of each epoch using a Keras callback (`DCGANMonitor`).  
- <b>Save & Load Models:</b> Trained generator models can be saved for future use.


## Steps

1. **Clone the repository** (or open the Colab notebook directly):

2. **Install required packages:**

3. **Dataset:**

<b><a href="https://www.kaggle.com/splcher/animefacedataset">Anime Face Dataset</a></b>

4. **Upload the dataset to Google Colab or your local environment.**

5. **Run the Notebook with T4 GPU (CPU takes forever).**

6. **Using the Generator:**
   
7. **After training, you can generate new images.**


