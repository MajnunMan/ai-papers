# How transferable are features in deep neural networks?

Yosinski, J., Clune, J., Bengio, Y., & Lipson, H. (2014). How transferable are features in deep neural networks? NIPS.

## Summary

When deep neural networks are trained the first layers learn the features which turn out not to be very specific to particular dataset or task but are very general to a lot of other datasets or tasks. These learned features eventually transition from being general to being specific to a dataset or task by the last layer of the deep neural network. This behavior of the deep neural networks has given birth to a powerful idea of applying knowledge that is gained from one task(base) to another task(target). To give an example, we can train a neural network to recognize objects like cats, dogs etc. and then use fully or partially that knowledge help us do a better job say reading x-ray scans. This is called transfer learning.
In real world an entire Convolutional Neural Network is trained is rarely trained from scratch with random parameter initialization. That is because not everyone has relatively sufficiently huge dataset to train the neural network. Instead the common approach is to pretrain a neural network on a large dataset, for example on ImageNet or COCO that contains millions of images with thousands of different objects of interest, and the use the Convolutional Neural Network either as an initialization or a fixed feature extractor for a particular computer vision task.
