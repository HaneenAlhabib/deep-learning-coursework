## CIFAR-10 Image Classification (Course Project)

This project implements image classification on the CIFAR-10 dataset
using transfer learning with a pretrained ResNet50 model.

This notebook was developed as part of a Deep Learning course assignment
and focuses on demonstrating correct training practices rather than
proposing a novel research contribution.

---

### Task
- Image classification
- 10 classes (CIFAR-10)

### Dataset
- CIFAR-10
- 60,000 color images (32×32)
- 50,000 training images, 10,000 test images

### Model
- Backbone: ResNet50 (pretrained on ImageNet)
- Framework: PyTorch
- Final classification layer adapted for CIFAR-10

### Training Details
- Data augmentation applied to training set
- Stratified train/validation split
- Loss function: Cross-Entropy
- Optimizer: Adam
- Learning rate scheduling
- Early stopping

### Results
- Validation Accuracy: ~97%
- Stable convergence without overfitting

### Notes
- This project is part of coursework and is included for completeness.
- The emphasis is on clean implementation and reproducibility.

---

## References

[1] A. Krizhevsky, “Learning Multiple Layers of Features from Tiny Images,” 2009.  
https://www.cs.toronto.edu/~kriz/cifar.html

[2] K. He et al., “Deep Residual Learning for Image Recognition,” CVPR 2016.  
https://arxiv.org/abs/1512.03385

[3] J. Yosinski et al., “How Transferable Are Features in Deep Neural Networks,” NeurIPS 2014.  
https://arxiv.org/abs/1411.1792

[4] PyTorch Documentation.  
https://pytorch.org/docs/stable/

[5] Torchvision Models.  
https://pytorch.org/vision/stable/models.html
