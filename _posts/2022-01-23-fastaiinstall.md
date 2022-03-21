---
layout: post
title: Fastaiv2 install
date: 2022-03-21
Author: SISI
categories: 
tags: [Fastai, install]

comments: true
--- 

Begin to work on fastai v2, so try to install it on GPU server

## Anaconda

First install anaconda on GPU server, then create a environment for fastaiv2.

## Pytorch and Fastai2

### First try install cuda11.2:

wget [https://developer.download.nvidia.com/compute/cuda/11.2.1/local_installers/cuda_11.2.1_460.32.03_linux.run](https://developer.download.nvidia.com/compute/cuda/11.2.1/local_installers/cuda_11.2.1_460.32.03_linux.run)

sudo sh cuda_11.2.1_460.32.03_linux.run

但是总是报错说我没有driver，其实用nvidia-smi看又是有的, this is not working.

### Install pytorch_gpu directly using conda

 conda install pytorch torchvision cudatoolkit=10.2 -c pytorch

### Conda install fastai2

conda install -c fastai  is to install  fastaiv2.5.3