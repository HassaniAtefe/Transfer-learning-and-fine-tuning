# Transfer-learning-and-fine-tuning

In this tutorial, you learn how to classify images of cats and dogs by using transfer learning from a pre-trained network (such as MobileNetV2).

 Summary :
* Using a pre-trained model for feature extraction: When working with a small dataset, it is a common practice to take advantage of features learned by a model trained on a larger dataset in the same domain. This is done by instantiating the pre-trained model and adding a fully-connected classifier on top. The pre-trained model is "frozen" and only the weights of the classifier get updated during training. In this case, the convolutional base extracted all the features associated with each image and you just trained a classifier that determines the image class given that set of extracted features.

* Fine-tuning a pre-trained model: To further improve performance, one might want to repurpose the top-level layers of the pre-trained models to the new dataset via fine-tuning. In this case, you tuned your weights such that your model learned high-level features specific to the dataset. This technique is usually recommended when the training dataset is large and very similar to the original dataset that the pre-trained model was trained on.

# Dataset
 a dataset containing several thousand images of cats and dogs.
 
# Acknowledgement
https://www.tensorflow.org/tutorials/images/transfer_learning
