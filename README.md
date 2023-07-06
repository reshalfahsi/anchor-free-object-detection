# Anchor-Free Object Detection


Anchor boxes have been the prevalent way to generate candidates for the ground truth bounding boxes in the object detection problem. Yet, this approach is such a hassle and downright confusing. This tutorial leverages an object detection method named [FastestDet](https://github.com/dog-qiuqiu/FastestDet) that is lightweight and anchor-free. ``PASCAL VOC 2007 and 2012`` datasets are utilized to evaluate the model's capability. Here, the train and validation set of both datasets is used for the train, validation, and test set in this tutorial with a ratio of ``81:9:10``. Eventually, the inference set (the test set of ``PASCAL VOC 2007``) is used to see the qualitative performance of the model.


## Experiment


Explore [here](https://github.com/reshalfahsi/anchor-free-object-detection/blob/master/AnchorFreeObjectDetection.ipynb) to execute training, testing, and inference.


## Result

## Quantitative Result

The table below presents the quantitative result of the model on the test set.

Test metric | PASCAL VOC 2007 & 2012
------------ | -------------
Loss |  3.026
mAP@0.5:0.95 | 21.5%


## Loss Curve

<p align="center"> <img src="https://github.com/reshalfahsi/anchor-free-object-detection/blob/master/assets/loss_curve.png" alt="loss_curve" > <br /> Loss curve on the train set and the validation set. </p>


## Qualitative Result

The qualitative results of the model on the inference set are shown below.

<p align="center"> <img src="https://github.com/reshalfahsi/anchor-free-object-detection/blob/master/assets/result00.png" alt="result00" > <br /> Three people are detected. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/anchor-free-object-detection/blob/master/assets/result01.png" alt="result01" > <br /> A boat and a person are detected. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/anchor-free-object-detection/blob/master/assets/result02.png" alt="result02" > <br /> A car is detected. </p>


## Credit

- [⚡FastestDet⚡](https://github.com/dog-qiuqiu/FastestDet)
- [GluonCV: a Deep Learning Toolkit for Computer Vision](https://cv.gluon.ai/contents.html)
- [Object Detection with RetinaNet](https://keras.io/examples/vision/retinanet/)
- [PyTorch Lightning](https://lightning.ai/docs/pytorch/latest/)
- [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/)
