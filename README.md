# Neural Style Transfer using Pretrained VGG19

This project implements **Neural Style Transfer (NST)** using **TensorFlow** and a **pretrained VGG19 model**.  
It combines the *content* of one image with the *style* of another image to create a visually appealing stylized output.



## Project Overview

Neural Style Transfer is a deep learning technique that uses a convolutional neural network (CNN) to blend two images:
- **Content Image:** Defines the structure and objects in the output.
- **Style Image:** Defines the texture, colors, and artistic patterns.

The pretrained **VGG19** model (trained on ImageNet) is used for feature extraction without additional training.



## Project Structure
```bash
├── data/
│   ├── content/            # Folder for content images
│   ├── style/              # Folder for style images
│
├── outputs/                # Stylized output images
│
├── scripts/
│   ├── utils.py            # Image loading, preprocessing, Gram matrix calculation
│   ├── style_transfer.py   # VGG19 model, loss functions, optimization logic
│
├── main.py                 # Entry point for executing style transfer
└── README.md               # Project documentation
```



## Features
- Uses **pretrained VGG19** model for feature extraction.
- Computes **content and style loss** for optimal blending.
- Performs **image optimization** using the Adam optimizer.
- Allows saving and viewing stylized output images.
- Handles resizing, normalization, and tensor preprocessing.



## Requirements

Install dependencies using pip:

```bash
pip install tensorflow numpy pillow matplotlib
```

## How to Run

1. Clone the Repository
git clone https://github.com/mokshas1/artisticstyletransfer.git
cd artisticstyletransfer

2. Upload Content and Style Images
Place them in:
data/content/
data/style/

3. Run the Program
python main.py

4. View Output
The stylized image will be displayed.

It will also be saved automatically in outputs/stylized_output.png.


## Tools & Frameworks Used

- TensorFlow / Keras – Neural network framework
- VGG19 – Pretrained CNN model from ImageNet
- Pillow (PIL) – Image loading and resizing
- NumPy – Array operations
- Matplotlib – Output visualization
