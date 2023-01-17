---
layout: page
title: Shallow-clouds
description: Understanding Clouds from Satellite Images
img: assets/img/shallow-clouds/shallow-clouds.png
# redirect: https://unsplash.com
importance: 1
category: work
---

[Shallow-clouds](https://gitlab.com/alt250/shallow-clouds): my solution to the Kaggle [Understanding Clouds from Satellite Images](https://www.kaggle.com/c/understanding_cloud_organization) competition.

I contributed a [Kaggle kernel](https://www.kaggle.com/alt250/multi-label-segmentation-using-fastai) with code to add multi-label image segmentation to the [fast.ai](https://docs.fast.ai) library

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/shallow-clouds/swath-gaps.png" title="Swath gaps" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Satellite imagery gaps present in the dataset
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/shallow-clouds/Conv-MCD.png" title="Conv-MCD" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

I implemented the multi-task [Conv-MCD](https://arxiv.org/abs/1908.05311) model

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/shallow-clouds/show-batch-with-masks.png" title="masks" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Examples of predicted masks
</div>
