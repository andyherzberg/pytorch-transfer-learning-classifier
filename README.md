# Pytorch Transfer Learning Classifier: To Bee or not to bee?

This Jupyter notebook is a Deep Learning transfer learning project that can be run on Google colab. The resulting model can differentiate between bees, wasps and humble bees. It was trained with about 60 images per class. See some random samples below. 

![train_dataset_batch1](https://github.com/andyherzberg/pytorch-transfer-learning-classifier/blob/master/img/Download.png)
![train_dataset_batch2](https://github.com/andyherzberg/pytorch-transfer-learning-classifier/blob/master/img/Download%20(1).png)
![train_dataset_batch3](https://github.com/andyherzberg/pytorch-transfer-learning-classifier/blob/master/img/Download%20(2).png)
![train_dataset_batch4](https://github.com/andyherzberg/pytorch-transfer-learning-classifier/blob/master/img/Download%20(3).png)
![train_dataset_batch5](https://github.com/andyherzberg/pytorch-transfer-learning-classifier/blob/master/img/Download%20(4).png)

I’m using the trained ResNet-50 Convolutional Neural network as the basis. The Convolutional Layers are freezed while the BatchNorm Layers are not as they shall work on the new image dataset. The classification block consists of 3 fully connected layers and finally a softmax function to calculate the class probabilities.
The notebook can be run on Google where all models, optimizer params and a log is stored. After training the classifier has an accuracy of approx. 95% on the unseen validation set. 

![train_dataset_batch5](https://github.com/andyherzberg/pytorch-transfer-learning-classifier/blob/master/img/Download%20(5).png)

The following images visualize the trained filters of the convolutional network.

<img src="https://github.com/andyherzberg/pytorch-transfer-learning-classifier/blob/master/img/Download%20(6).png" width="70%">
