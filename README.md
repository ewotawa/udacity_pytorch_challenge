# udacity_pytorch_challenge
Jupyter (Google Colab) notebook and model definition for Facebook Udacity Pytorch Challenge project

The purpose of this repository is to house the assets for my Udacity PyTorch Challenge project. 

## Assignment
The assignment is to build a neural network to perform image classification, specifically, to identify flower species from photos of flowers passed in to the model. Udacity provided the image set on which I trained the model. 

## Neural Network
I used a pretrained neural network optimized for the identification of features associated with image classification. I chose to use the VGG16 neural network. Because VGG16 is trained on the ImageNet dataset, I needed to train a different classifier so that the model could understand the images I was passing to it. I therefore wrote and trained an image classifier to use alongside the frozen feature identifiers from the VGG16 model

## Checkpoint
After I trained the model, I saved a checkpoint so that I wouldn't have to retrain the model every time I went back to the notebook. That file also is stored in this repo so that you can load it yourself: 
```
trained_vgg16_classifier.pt
```

## Model output
The assignment was to construct a function that could take in an image and a model and produce the five most likely flower species along with the probabilities of each. I also prepared a more user-friendly version of the output so that the user can see:
* the passed-in image
* a bar graph with the most likely flower species and their probabilities
* text labels for the species names instead of the key values for them on which the model trained.
