# CIFAR-10 Image Classification
## About
This project uses a CNN with an Inception-style module to classify CIFAR-10 images into 10 classes. It studies the effects of data augmentation, regularization, and Test-Time Augmentation (TTA).
## Dataset
- Dataset: CIFAR-10
- Training images: 400
- Validation images: 100
- Test images: 10,000
- Classes: 10

## Technologies
- Python
- TensorFlow/Keras
- NumPy
- Matplotlib
- Scikit-learn

## How to Run
**1. Clone the repository**
git clone <YOUR_REPOSITORY_URL>
cd <YOUR_REPOSITORY_NAME>
**2. Install the required libraries**
pip install tensorflow numpy pandas matplotlib scikit-learn scipy jupyter
**3. Open the notebook**
Open `DL_ASS01_23F_0515.ipynb` and run all cells in order.
(The CIFAR-10 dataset will be downloaded automatically)
## Experiments
- Baseline CNN without augmentation
- Geometric and photometric augmentation
- Random Erasing and Mixup
- Regularization techniques
- Clean, shifted, and grayscale image evaluation
- Test-Time Augmentation (TTA)

## Reproduce the random selections
The notebook sets random seeds, including 42 for the initial data selection and 42, 123, and 2026 for the multi-seed experiments.
Results can still vary slightly across hardware, TensorFlow versions, and execution environments. For the closest reproduction, use the same notebook, dependency versions, random seeds, and execution order.
## Results
The experiments compare model accuracy under different settings. Geometric and photometric augmentation performed better on shifted images than the baseline, but overall accuracy remained limited due to the small training dataset.
