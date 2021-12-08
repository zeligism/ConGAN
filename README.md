# Improving Latent Space of GANs

[Abdulla Jasem Ahmed Jaber Almansoori](https://github.com/zeligism/), [Talal Abdullah Fadhl Algumaei](https://github.com/Talal-Algumaei), [Muhammad Hamza Sharif](https://github.com/Sharifmhamza/)

[![PWC](https://img.shields.io/badge/State--of--the--Art-Self--supervised--Learning%3A%20Generative%20or%20Contrastive-green?style=flat&logo=flat)](https://arxiv.org/abs/2006.08218)
[![PWC](https://img.shields.io/badge/State--of--the--Art-Auto--Encoding%20Variational%20Bayes-green?style=flat&logo=flat)](https://arxiv.org/abs/1312.6114)
[![PWC](https://img.shields.io/badge/State--of--the--Art-Generative%20Adversarial%20Network-green?style=flat&logo=flat)](https://paperswithcode.com/paper/generative-adversarial-networks)
[![PWC](https://img.shields.io/badge/State--of--the--Art-Info--Gan-green?style=flat&logo=flat)](https://paperswithcode.com/method/infogan)
[![PWC](https://img.shields.io/badge/State--of--the--Art-Exploring--Simple--Siamese--Representation-green?style=plastic&logo=flat)](https://paperswithcode.com/paper/exploring-simple-siamese-representation)

## Introduction
The repository contains the implementation of improving latent space of GANs. In this project, we are combining three learning paradigms: generative learning,
contrastive learning, and generative-contrastive learning. Our main objective is to train GAN to learn disentangled representations. For that purpose, we proposed two frameworks.
### Proposed Framework 1:
In the first proposed framework, we combined GANs, SimSam Network and Autoenconder. The architecture of proposed framework is shown as: 

<img src="Architecture/Proposed_FrameWork_1.png" style="display:block;float:none;margin-left:50;margin-right:50;width:60%">

### Proposed Framework 2:
In the second proposed framework, we used Info-GAN with spectral normalization and condition it using the representation from SimSam Network. The architecture of proposed framework is shown as:

<img src="Architecture/Proposed_FrameWork_2.jpg" style="display:block;float:none;margin-left:50;margin-right:50;width:80%">
The second framework performs better, we use it to run the experiment and compile the results.

## Dependencies
* Ubuntu based machine with NVIDIA GPU or GoogleColab is required to run the training and evaluation.
* Python 3.8.
* Pytorch 1.10.0+cu111 and corresponding torchvision version.

## Installation
It is recommended to create a new conda environment for this project. The installation steps are as follows:
1. Create new conda environment and activate it.
```bash
$ conda create --name=ConGAN python=3.8
$ conda activate ConGAN
```
2. Install requirements as,
```bash
$ pip install -r requirements.txt
```
## Training Model from Strach
For training the model from strach for this project, it is recommended to follow the following steps:
1. Create the new folder name **gansiam** in your machine.
2. Extract all files of this repository in **gansiam** folder.
3. Download the pretrained model of SimSam network with 256 batch size and 100 epoches from this [link](https://github.com/facebookresearch/simsiam).
4. Put the pretrained model in your gansiam folder and rename as: **pretrained_batch256.tar**.
5. Change the path of **GANSIAM_DIR** it [jupyter notebook](https://github.com/zeligism/ConGAN/blob/main/ConsistentGAN.ipynb) with the path of your folder **gansiam**.

## Evaluating the pretrained-model


## Contact
Should you have any question, please create an issue on this repository or contact at Abdulla.Almansoori@mbzuai.ac.ae, Talal.Algumaei@mbzuai.ac.ae, Muhammad.Sharif@mbzuai.ac.ae

