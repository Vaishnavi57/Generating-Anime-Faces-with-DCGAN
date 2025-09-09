# Anime Faces Generation with DCGAN

<p align="center">
  <img src="outputs/Screenshot 2025-09-09 183853.png" alt="Sample Anime Faces" width="400"/>
</p>

**Description:**  
This project implements a <b>Deep Convolutional Generative Adversarial Network (DCGAN)</b> to generate realistic anime face images. Built with <b>TensorFlow</b> and <b>Keras</b>, it demonstrates how GANs learn to produce images from random noise vectors.

---

## Project Overview

- <b>Generator:</b> Converts random noise vectors into 64×64 RGB anime face images using Dense, Conv2DTranspose, and ReLU layers.  
- <b>Discriminator:</b> Distinguishes real vs. generated images using Conv2D, MaxPooling2D, and LeakyReLU layers.  
- <b>DCGAN Class:</b> Combines Generator and Discriminator with custom training steps.  
- <b>Visualization:</b> Generates and displays sample images at the end of each epoch using a Keras callback (`DCGANMonitor`).  
- <b>Save & Load Models:</b> Trained generator models can be saved for future use.

---

## Project Structure


---

## Getting Started

1. **Clone the repository** (or open the Colab notebook directly):

```bash
git clone https://github.com/<USERNAME>/Anime-DCGAN.git
cd Anime-DCGAN
```

##Install required packages:
```bash

pip install tensorflow numpy matplotlib seaborn pillow
```



##Dataset:

####Use the <a href="https://www.kaggle.com/splcher/animefacedataset">Kaggle Anime Face Dataset</a>.

####Upload the dataset to Google Colab or your local environment.

###Run the Notebook:

####Open DCGAN_Anime.ipynb in Colab.

####Run all cells to train the model and generate sample images.

##Using the Generator:
####After training, you can generate new images:
```bash

from tensorflow.keras.models import load_model
import tensorflow as tf

generator = load_model("DCGAN_Generator.h5")
random_noise = tf.random.normal([10, 300])
generated_images = generator(random_noise)
```
