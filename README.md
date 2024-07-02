# Human Pose Estimation

Welcome to the Human Pose Estimation project!.

## Project Overview

In this project, we modify the last layer of the ResNet-50 model to adapt it for the Human Pose Estimation task. We apply these modifications to a dataset of 700 CCTV images, aiming to accurately estimate human poses.

## Getting Started

### Prerequisites

Ensure you have the following dependencies installed:
* Python 3.x
* PyTorch
* torchvision
* numpy
* matplotlib
* tqdm
* PIL (Pillow)

### Installation

Clone the repository and install the required packages:

```bash
git clone https://github.com/yourusername/Human_pose_estimation.git
cd Human_pose_estimation
pip install -r requirements.txt

```

### Dataset
The dataset consists of 700 CCTV images annotated for human pose estimation. The images and their annotations are stored in the following structure:

``` bash /path/to/dataset/
    Images/
        image1.jpg
        image2.jpg
        ...
    CCTVAnnotations.json
```

### Model
The model used in this project is a modified ResNet-50. We replace the final layer to predict 17 keypoints (each with x, y coordinates and visibility).
Training
To train the model, run:

``` bash
python train.py --dataset /path/to/dataset --epochs 100

```

During training, progress bars will show the training and validation process. The training and validation losses will be plotted at the end of the training.
 ### Future Work

1. Experiment with different models to improve accuracy.
2. Explore MediaPipe for real-time pose estimation.
3. Investigate YOLO and other zero-shot models for human pose estimation.


### Contributing
Contributions are welcome! Please open an issue or submit a pull request.
### License
This project is licensed under the MIT License.

