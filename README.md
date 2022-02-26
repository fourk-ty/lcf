# PyTorch implementation for the TGRS paper: "Label Noise Modeling and Correction via Loss Curve Fitting for SAR ATR

We are planning to open our code for the paper: Label Noise Modeling and Correction via Loss Curve Fitting for SAR ATR. 

The success of deep learning in synthetic aperture radar (SAR) automatic target recognition (ATR) relies on a large number of labeled samples; however, there are often wrong (noisy) labels in a large-scale dataset. In this article, we propose a loss curve-fitting-based method, which can identify the noisy labels and train the classification network effectively. We propose to model label noise by unsupervised clustering via fitting loss curve to identify whether the sample’s label is clean or noisy. Then, we train the network using augmented samples with clean labels to correct noisy labels further. The experiments on the moving and stationary target acquisition and recognition (MSTAR) dataset prove that our proposed method can deal with the situation when training a network with different ratios of noisy labels and correct noisy labels effectively. When the noise ratio is small (40%) in the training dataset, our method can correct 97.9% of noisy labels and train the classification network with 98.8% classification accuracy. While the noise ratio is large (80%), our method can correct 78.1% of noisy labels and train the classification network with 79.6% classification accuracy.

![image](https://github.com/fourk-ty/any_images/blob/main/loss-curve%40per-sample-paper.jpg)
![image](https://github.com/fourk-ty/any_images/blob/main/plt_show_correction%40400.jpg)

If the code is helpful, please consider to cite our paper

```latex
@ARTICLE{9580898,
author={Wang, Chen and Shi, Jun and Zhou, Yuanyuan and Li, Liang and Yang, Xiaqing and Zhang, Tianwen and Wei, Shunjun and Zhang, Xiaoling and Tao, Chongben},
journal={IEEE Transactions on Geoscience and Remote Sensing}, 
title={Label Noise Modeling and Correction via Loss Curve Fitting for SAR ATR}, 
year={2022},
volume={60},
number={},
pages={1-10},
doi={10.1109/TGRS.2021.3121397}}
```

We would like to thank the authors (Eric Arazo, Diego Ortego, Paul Albert, Noel E O'Connor, and Kevin McGuinness) of the paper "Unsupervised Label Noise Modeling and Loss Correction" with [code](https://github.com/PaulAlbert31/LabelNoiseCorrection). Our implementation environment is similar to the code. You can cite their work as follows.

```latex
 @inproceedings{ICML2019_UnsupervisedLabelNoise,
  title = {Unsupervised Label Noise Modeling and Loss Correction},
  authors = {Eric Arazo and Diego Ortego and Paul Albert and Noel E O'Connor and Kevin McGuinness},
  booktitle = {International Conference on Machine Learning (ICML)},
  month = {June},
  year = {2019}
 }
```

[1] Eric Arazo*, Diego Ortego*, Paul Albert, Noel E. O'Connor, Kevin McGuinness, Unsupervised Label Noise Modeling and Loss Correction, International Conference on Machine Learning (ICML), 2019
