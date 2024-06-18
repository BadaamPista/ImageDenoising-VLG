

## Overview

This project explores the use of the U-Net model for image denoising. The U-Net architecture is chosen for its effectiveness in restoring noisy images while preserving fine details. This `README.md` provides an overview of the project, its setup, implementation details, and outcomes.

## Setup

### Requirements

- Python 3.x
- TensorFlow 2.x
- NumPy
- OpenCV (cv2)
- Matplotlib (for visualization)

### Installation

1. Clone the repository:

   ```bash
   git clone {github_url}
   cd {project_name.lower().replace(" ", "-")}

Implementation:

Dataset

The dataset used in this project consists of pairs of noisy images (low_images) and their corresponding clean versions (high_images). Ensure the dataset is structured as follows:

   dataset/
├── low_images/
│   ├── image1.png
│   ├── image2.png
│   └── ...
└── high_images/
    ├── image1.png
    ├── image2.png
    └── ...

Model Architecture

The U-Net model architecture used for image denoising is implemented using TensorFlow/Keras. The model consists of an encoder-decoder structure with skip connections to preserve spatial information.

Training
Adjust the parameters in config.py for batch size, learning rate, and other training settings.

Train the model:

python train.py

Evaluation

After training, evaluate the model using validation data to compute metrics such as Peak Signal-to-Noise Ratio (PSNR), Mean Squared Error (MSE), and Mean Absolute Error (MAE):

Results

PSNR: 19.65157681772904
