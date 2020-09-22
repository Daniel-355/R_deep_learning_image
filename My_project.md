# Using transfer learning to classify pictures of pathology of colorectal cancer
[TOC]
## Data sources  

These pictures have been labeled by pathologists at the University Hospitals Coventry and Warwickshire ![link]((https://warwick.ac.uk/fac/sci/dcs/research/tia/glascontest/download/)), which included two classifications: benign (74) and malignant (91). All 165 pictures were split into two datasets: training dataset (85) and test dataset (80). 
The composition of the dataset is as follows.
Split	|Warwick-QU
----|----
Training	| benign : 37
||malignant : 48
Test	|benign : 37
||malignant : 43  

Tabel of classification of colorectal cancer  
![Tabel of classification of colorectal cancer](https://github.com/Daniel-355/R_deep_learning_image/blob/master/Picture1.png?raw=true)  
 
Sample of picture  
![Sample of picture](https://github.com/Daniel-355/R_deep_learning_image/blob/master/Picture2.png?raw=true )  

## Data processing
* Transform all pictures to "tfrecord" file so that Colab can read these data. (xml-- csv --tfrecord , train_images, train_labels, test)
* _I will learn how to load my own dataset into Colab_ ![link](https://colab.research.google.com/github/tensorflow/docs-l10n/blob/master/site/zh-cn/tutorials/load_data/images.ipynb#scrollTo=n2TCr1TQ8pA3). 

## Transfer learning with tensorflow hub according to this ![website](https://colab.research.google.com/github/tensorflow/docs/blob/master/site/en/tutorials/images/transfer_learning_with_hub.ipynb#scrollTo=CKFUvuEho9Th). 
* Download the classifier 
* Load my dataset
* Run the classifier on a batch of images
* Download the headless model
* Attach a classification head
* Train the model
* Check the predictions and evaluate the model
* Compare the effect of different classifier, like mobilenet, inception v3,,,
* Export the model 

## Build a convolutional neural network according to below ![websites](https://www.tensorflow.org/tutorials/images/classification#visualize_training_results_2 )  and ![link](https://colab.research.google.com/github/tensorflow/docs-l10n/blob/master/site/zh-cn/tutorials/images/cnn.ipynb#scrollTo=_v8sVOtG37bT).  (if possible)

sampling

## Compare the effect of convolutional neural network, and neural network.  (if possible)

# Questions:
* I am not sure whether I can finish the above analysis by using only Colab. If not, I may need set up a enivironment the transfer learning. 
* My person computer is competent or not. 
* How to prepare a well dataset for Colab. 
* The training smample size my be not enough. 
 
	

