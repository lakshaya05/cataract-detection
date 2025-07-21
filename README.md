# Cataract Detection using SIFT and GLCM

## Table of Contents

- [Introduction](#introduction)
- [Methodology](#methodology)
  - [SIFT](#sift)
  - [GLCM](#glcm)
- [Installation](#installation)
- [Usage](#usage)
- [Google Colab](#google-colab)
- [Dataset](#dataset)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project focuses on automatic detection of cataracts using image processing techniques, specifically leveraging **SIFT** (Scale-Invariant Feature Transform) and **GLCM** (Gray Level Co-occurrence Matrix). By extracting key features from eye images and training a model, the system aims to classify whether an eye is affected by cataracts.

## Methodology

The project employs two key techniques for feature extraction:

### SIFT

SIFT is a well-known algorithm for detecting and describing local features in images. In this project, SIFT is used to extract the most important keypoints from eye images, capturing important structural information about the eye’s lens.

### GLCM

GLCM is used to capture textural features in an image by considering the spatial relationships between pixel intensities. In this project, we use GLCM to extract textural features from the eye images, which are then used in conjunction with SIFT features to enhance the classification.

## Installation

Follow these steps to set up the project:

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/cataract-detection.git
    ```

2. Navigate to the project directory:

    ```bash
    cd cataract-detection
    ```


## Usage

1. Prepare the dataset by placing the images in the `mypath` .
2. Run the feature extraction and classification script:

    ```bash
    python main.py
    ```

3. The results will be displayed, showing whether the images indicate the presence of cataracts.

## Google Colab

You can also run this project directly on Google Colab without needing to install anything locally. Just click the link below:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/10FrM9Yv5J9XxGP_Fb26FPaYyJausxlrF?usp=sharing)

This Colab notebook provides an interactive way to test the model, run experiments, and visualize results using a preconfigured environment in the cloud.

## Dataset

The dataset used for this project consists of eye images, including both healthy and cataract-affected eyes. If you'd like to use a custom dataset, you can place the images in the `data/` directory with appropriate labels.

**Note:** Make sure the dataset is preprocessed (resized, normalized) according to the model’s input requirements.

## Results

After processing the images through SIFT and GLCM, the features are classified using a machine learning model. Here are some sample results:

| Image           | Predicted Class   |
| --------------- | ----------------- |
| eye_image_1.jpg | Cataract Detected  |
| eye_image_2.jpg | No Cataract        |

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


