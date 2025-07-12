# MoGe: Accurate Monocular Geometry Estimation for Open-Domain Images

![MoGe Logo](https://img.shields.io/badge/MoGe-3D%20Reconstruction-brightgreen) ![CVPR'25](https://img.shields.io/badge/CVPR'25-Oral%20Presentation-blue)

[![Download Releases](https://img.shields.io/badge/Download%20Releases-Click%20Here-orange)](https://github.com/HWDHirushan/MoGe/releases)

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Training](#training)
- [Evaluation](#evaluation)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Overview

MoGe stands for Monocular Geometry Estimation. This project focuses on enhancing the accuracy of monocular depth estimation for open-domain images. It provides an optimal training supervision method that unlocks new possibilities in 3D reconstruction and monocular vision tasks.

The method is designed to address challenges in monocular depth estimation by using innovative techniques that leverage existing datasets and improve performance metrics significantly.

## Key Features

- **Accurate Depth Estimation**: Achieves state-of-the-art results in monocular depth estimation.
- **Open-Domain Capability**: Works effectively on diverse datasets, adapting to various scenes and environments.
- **Optimal Training Supervision**: Utilizes advanced training techniques for improved model performance.
- **3D Reconstruction**: Facilitates the reconstruction of 3D models from 2D images, enhancing applications in computer vision.

## Installation

To get started with MoGe, follow these steps to set up your environment:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/HWDHirushan/MoGe.git
   cd MoGe
   ```

2. **Install Dependencies**:
   Make sure you have Python 3.7 or higher. You can create a virtual environment and install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download Pre-trained Models**:
   Visit the [Releases section](https://github.com/HWDHirushan/MoGe/releases) to download the necessary files. Follow the instructions provided there to set up the pre-trained models.

## Usage

Once the installation is complete, you can start using MoGe for your monocular geometry estimation tasks.

1. **Run the Model**:
   Use the following command to run the model on your images:
   ```bash
   python run_moge.py --input <path_to_image> --output <path_to_output>
   ```

2. **Visualize Results**:
   The output will include depth maps and reconstructed 3D models. You can visualize them using tools like Open3D or Matplotlib.

## Dataset

MoGe can be trained on various datasets. Some recommended datasets include:

- **KITTI**: A popular dataset for stereo and monocular depth estimation.
- **NYU Depth V2**: Provides RGB-D images for indoor scenes.
- **Cityscapes**: Useful for urban scene understanding.

Ensure that the dataset is properly formatted as per the requirements specified in the repository.

## Training

To train the model on your dataset, follow these steps:

1. **Prepare Your Dataset**:
   Ensure your dataset is organized correctly. You may need to create a configuration file that specifies the paths to your training and validation datasets.

2. **Start Training**:
   Run the training script with the following command:
   ```bash
   python train.py --config <path_to_config_file>
   ```

3. **Monitor Training**:
   Use TensorBoard to monitor the training process. You can start TensorBoard with:
   ```bash
   tensorboard --logdir logs/
   ```

## Evaluation

After training, evaluate the model's performance on a validation set. Use the evaluation script provided in the repository:

```bash
python evaluate.py --model <path_to_trained_model> --data <path_to_validation_data>
```

This will output performance metrics such as RMSE and MAE, allowing you to assess the model's accuracy.

## Contributing

Contributions are welcome! If you want to improve MoGe, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch and create a pull request.

Please ensure that your code adheres to the project's coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgments

We would like to thank the contributors and researchers who made this project possible. Special thanks to the authors of the datasets used and the tools that support this work. 

For further details and to download the latest releases, visit the [Releases section](https://github.com/HWDHirushan/MoGe/releases).