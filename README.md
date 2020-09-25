# GAN-food-image-generator
Use GANs to generate food images (with Kaggle's Food-101 dataset)


**Original paper**

I. J. Goodfellow et al. (2014) **Generative Adversarial Nets** [[arXiv]](https://arxiv.org/abs/1406.2661)

---
## Model Atchitecture

#### The Generator

The generator consists of 4 fully connected layers:

**FC1**: 256 units, LeakyReLU activation with alpha = 0.1, and batch normalizaion with momentum = 0.8

**FC2**: 512 units, LeakyReLU activation with alpha = 0.1, and batch normalizaion with momentum = 0.8

**FC3**: 512 units, LeakyReLU activation with alpha = 0.1, and batch normalizaion with momentum = 0.8

**FC4 (output layer)**: h*w*3 units (the size of the fake image, including the rgb dimension) and the **tanh** activation


#### The Discriminator

The discrimanator consists of 3 fully connected layers:

**FC1**: 256 units, LeakyReLU activation with alpha = 0.1, and dropout with rate = 0.2

**FC2**: 256 units, LeakyReLU activation with alpha = 0.1, and dropout with rate = 0.2

**FC3 (output layer)**: 1 unit and the **sigmoid** activation

#### Hyperparameters


### Result

