# CIFAR-10 Image Classification: Custom CNN vs. ResNet18

A comparative study on object recognition using a scratch-built Convolutional Neural Network and Transfer Learning via ResNet18.

## 📊 Results Comparison
| Model | Overall Accuracy | "Cat" Class Accuracy |
| :--- | :--- | :--- |
| **Custom CNN (3-Layer)** | 80.4% | 61.7% |
| **ResNet18 (Transfer Learning)** | **93.5%** | **83.5%** |

## 🚀 Key Technical Implementation
- **Architecture:** Transitioned from a standard 3-layer CNN to a Residual Network (ResNet) to solve the vanishing gradient problem.
- **Data Augmentation:** Used `RandomHorizontalFlip` and `RandomRotation` to improve generalization.
- **Fine-Tuning:** Implemented a two-phase training strategy (freezing/unfreezing layers) to maximize pre-trained feature extraction.
- **Hardware:** Accelerated via **NVIDIA RTX 5060 (CUDA)**.

## 🛠️ How to Run
1. Clone the repo.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run `cifar10_cnn.ipynb` for the scratch model.
4. Run `resnet_transfer_learning.ipynb` for the ResNet model.
