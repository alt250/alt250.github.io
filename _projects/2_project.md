---
layout: page
title: Sparse train
description: Fast neural network training by dynamic sparsification
img: assets/img/sparse-train/conv_ch_pruning.png
# redirect: https://unsplash.com
importance: 1
category: work
---
Fast implementation of [PruneTrain: Fast Neural Network Training by Dynamic Sparse Model Reconfiguration](https://arxiv.org/abs/1901.09290) to reduce training time.

Modify the model architecture during training by removing entire convolutional layers for GPU mechanical sympathy, see [here](https://gitlab.com/alt250/sparse-train/-/blob/master/report/_book/_main.pdf) for details.

[Project code](https://gitlab.com/alt250/cifar10-fast)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/sparse-train/conv_ch_pruning.png" title="Conv channel pruning" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
Example of convolution layer channel pruning ([source](https://machinethink.net/blog/compressing-deep-neural-nets/))

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/sparse-train/vgg16_dense_sparse_acc_2.png" title="accuracy of sparse model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
Sparse models trained from scratch preserve classification performance.

A smaller model is created as a by-product of sparse training. This is an improvement over other methods which re-train a pre-trained model to induce sparsity and compress it.

The sparsified model has lower parameters and resources requirements, so it is more feasible to deploy it on hardware with limited memory. Also, more instances can then deployed in parallel in a production environment, allowing for greater scalability.
