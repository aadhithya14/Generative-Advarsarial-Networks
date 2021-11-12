#Wassertian GAN

The Wasserstein GAN, or WGAN for short, was introduced by Martin Arjovsky, et al. in their 2017 paper titled “Wasserstein GAN.” [Paper](https://arxiv.org/abs/1701.07875)


It is an extension of the GAN that seeks an alternate way of training the generator model to better approximate the distribution of data observed in a given training dataset.

Instead of using a discriminator to classify or predict the probability of generated images as being real or fake, the WGAN changes or replaces the discriminator model with a critic that scores the realness or fakeness of a given image.This change is motivated by a theoretical argument that training the generator should seek a minimization of the distance between the distribution of the data observed in the training dataset and the distribution observed in generated examples.
The benefit of the WGAN is that the training process is more stable and less sensitive to model architecture and choice of hyperparameter configurations. It is less prone to mode collapse than other types of GANs. Perhaps most importantly, the loss of the discriminator appears to relate to the quality of images created by the generator.

This repository contains clean implementation of WGAN to generate images of handwritten digits.

![results](https://user-images.githubusercontent.com/50480450/141417577-453f307c-5178-4160-ad93-3468e1a785f5.png)


