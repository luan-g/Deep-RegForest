# Deep Regression Forests

Code accompanying the paper **Deep Regression Forests for Age Estimation**.
For detailed algorithm and experiment results please see our CVPR 2018 [paper](https://arxiv.org/abs/1712.07195).

## How to use

1. Download the Morph dataset. The Morph dataset is not free availabel, but you can request for it from [here](https://ebill.uncw.edu/C20231_ustores/web/store_main.jsp?STOREID=4).
2. Download pre-trained VGG model [VGG_ILSVRC_16_layers.caffemodel](http://www.robots.ox.ac.uk/~vgg/software/very_deep/caffe/VGG_ILSVRC_16_layers.caffemodel) .
3. Create a symbolic link to the Morph dataset with the name 'data/morph'.

    `ln -s 'the directory for Morph dataset' data/morph`
4. Create the train set list and test set list.

    `python split.py`
5. Start to train.

    `python run.py`
