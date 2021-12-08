# Improving Latent Space of GANs

[Abdulla Jasem Ahmed Jaber Almansoori](https://github.com/zeligism/), [Talal Abdullah Fadhl Algumaei](https://github.com/Talal-Algumaei), [Muhammad Hamza Sharif](https://github.com/Sharifmhamza/)

[![PWC](https://img.shields.io/badge/State--of--the--Art-Self--supervised--Learning%3A%20Generative%20or%20Contrastive-green?style=flat&logo=flat)](https://arxiv.org/abs/2006.08218)
[![PWC](https://img.shields.io/badge/State--of--the--Art-Auto--Encoding%20Variational%20Bayes-green?style=flat&logo=flat)](https://arxiv.org/abs/1312.6114)
[![PWC](https://img.shields.io/badge/State--of--the--Art-Generative%20Adversarial%20Network-green?style=flat&logo=flat)](https://paperswithcode.com/paper/generative-adversarial-networks)
[![PWC](https://img.shields.io/badge/State--of--the--Art-Info--Gan-green?style=flat&logo=flat)](https://paperswithcode.com/method/infogan)
[![PWC](https://img.shields.io/badge/State--of--the--Art-Exploring--Simple--Siamese--Representation-green?style=plastic&logo=flat)](https://paperswithcode.com/paper/exploring-simple-siamese-representation)

## Introduction
The repository contains the implementation of improving latent space of GANs. In this project, we are combining three learning paradigms: generative learning,
contrastive learning, and generative-contrastive learning. Our main objective is to learn GAN disentangled representations.
### Proposed Framework 1:
In the first proposed framework, we combined GANs, SimSam Network and Autoenconder. The architecture of proposed framework is shown in [Figure](https://github.com/zeligism/ConGAN/tree/main/Architecture).
### Proposed Framework 2:
In the second proposed framework, we used Info-GAN with spectral normalization and condition it using the representation from SimSam Network. The architecture of proposed framework is shown in [Figure](https://github.com/zeligism/ConGAN/tree/main/Architecture).

## Dependencies
* Ubuntu based machine with NVIDIA GPU or GoogleColab is required to run the training and evaluation.
* Python 3.8.
* Pytorch 1.10.0+cu111 and corresponding torchvision version.

## Installation
It is recommended to create a new conda environment for this project. The installation steps are as follows:
1. Create new conda environment and activate it.
```bash
$ conda create --name=gansiam python=3.8
$ conda activate gansiam
```
2. Install requirements as,
```bash
$ pip install -r requirements.txt
```




