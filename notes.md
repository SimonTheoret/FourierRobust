# Paper: A Fourier Perspective on Model Robustness in Computer Vision
[Paper](https://arxiv.org/pdf/1906.08988.pdf)
## Main insights

- Gaussian data augmentation and adversarial training bias models towards low
  frequency information
- Adversarial examples are not strictly a high frequency phenomenon
- Fourier perspective is not predictive in all situations of transfer between
  data augmentation and robustness.
- More varied data augmentation offers more general robustness

### Quotes
Second, the fact that adversarial training biases these perturbations towards the lower frequencies
suggests an intriguing connection between adversarial training and the DeepViz method for
feature visualization. In particular, optimizing the input in the low frequency domain is one of the
strategies utilized by DeepViz to bias the optimization in the image space towards semantically
meaningful directions. Perhaps the reason adversarially trained models have semantically meaningful
gradients is because gradients are biased towards low frequencies in a similar manner as utilized
in DeepViz.


# Paper: When Adversarial Training Meets Vision Transformers: Recipes from Training to Architecture
[Paper](https://arxiv.org/pdf/2210.07540.pdf)
## Main insights
- We find that pre-training and SGD optimizer are necessary for ViTs’
  adversarial training.


# Paper: Imagenet-trained CNNs are biased towards texture
[Paper](https://arxiv.org/pdf/1811.12231.pdf)
## Main insights
- We show that ImageNettrained CNNs are strongly biased towards recognising
  textures rather than shapes
- Increasing shape bias implies improved object detection performance and
  previously unseen robustness towards a wide range of image distortions,
  highlighting advantages of a shape-based representation.

# Paper: Fourier Sensitivity and Regularization of Computer Vision Models
[Paper](https://openreview.net/pdf?id=VmTYgjYloM)
## Main insights
- Formalize formalize models' sensitivity to features frequency (called Fourier
  sensitivity)
  - Fourier-sensitivity is a measure of the relative magnitudes of a model’s
    inputgradient with respect to different frequency bands in the input
    spectrum
- Propose Fourier regularization to modify the Fourier sensitivity of their
  models
- Adversarial training implies a radically different sensitivity in ResNet50
- Gaussian augmentation implies a slightly different sensitivity in ResNet50
- Sensitivity computed on ImageNet, CIFAR10 and SVHN
