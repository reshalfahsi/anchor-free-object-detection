# Anchor-Free Object Detection


 <div align="center">
    <a href="https://colab.research.google.com/github/reshalfahsi/anchor-free-object-detection/blob/master/AnchorFreeObjectDetection.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="colab"></a>
    <br />
 </div>


Anchor boxes have been the prevalent way to generate candidates for the ground truth bounding boxes in the object detection problem. Yet, this approach is such a hassle and downright confusing. This tutorial leverages an object detection method named [FastestDet](https://github.com/dog-qiuqiu/FastestDet) that is lightweight and anchor-free. ``PASCAL VOC 2007 and 2012`` datasets are utilized to evaluate the model's capability. Here, the train and validation sets of ``PASCAL VOC 2012`` are used for the train, validation, and test set in this tutorial with a ratio of ``81:9:10``. Eventually, the inference set (the test set of ``PASCAL VOC 2007``) is used to see the qualitative performance of the model.


## Experiment


Explore [here](https://github.com/reshalfahsi/anchor-free-object-detection/blob/master/AnchorFreeObjectDetection.ipynb) to execute training, testing, and inference.


## Result

## Quantitative Result

The table below presents the quantitative result of the model on the test set.

Test metric | PASCAL VOC 2012
------------ | -------------
Loss |  2.331
mAP@0.5:0.95 | 25.560%


## Loss Curve

<p align="center"> <img src="https://github.com/reshalfahsi/anchor-free-object-detection/blob/master/assets/loss_curve.png" alt="loss_curve" > <br /> Loss curve on the train set and the validation set. </p>


## Qualitative Result

The qualitative results of the model on the inference set are shown below.

<p align="center"> <img src="https://github.com/reshalfahsi/anchor-free-object-detection/blob/master/assets/qualitative_result.png" alt="qualitative_result" > <br /> A person, a motorbike (left), a bird (middle), and two TV monitors (right) are detected. </p>


## Credit

- [⚡FastestDet⚡](https://github.com/dog-qiuqiu/FastestDet)
- [GluonCV: a Deep Learning Toolkit for Computer Vision](https://cv.gluon.ai/contents.html)
- [Object Detection with RetinaNet](https://keras.io/examples/vision/retinanet/)
- [PyTorch Lightning](https://lightning.ai/docs/pytorch/latest/)
- [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/)
