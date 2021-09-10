# ML
Machine Learning Projects - by Shubham Kaushal

## MNIST handwritten image classifier | Supervised Learning | 2021
MNIST 784 data is a collection of 70,000 labeled images of handwritten digits from 0 to 9. Each digit is represented by a 28x28 2D array (i.e., 784 columns), and it is divided into training and testing sets (60000 and 10000). This dataset is widely used for training and testing various image processing systems. 

The task is classification/predicting which digit each image represents by matching it to its label. The present error rate (without deskewing/shiftable edges or using neural networks) is 2.8%* using a single model. Here I have tried to build a stack of models, with each layer training on the previous layer’s output.

Models tested
<ul>
  <li>ElasticNet
  <li>SGDRegressor
  <li>KNeighborsClassifier
  <li>RandomForestClassifier
  <li>AdaBoostClassifier
</ul>

Final Choice of Classifier: KNeighborsClassifier <br>
Accuracy Achieved: 96.91%

Data Augmentation <br>
Data Augmentation is a technique in data analysis to artificially increase the amount of data by adding slightly modified copies of existing data. This is done by allowing small translation, rotation, cropping of the images. Here 1 unit translation is used in all four directions. <br>
Accuracy Achieved: 97.66%

Stacking Models <br>
A custom two-layer classifier using RandomForest, KNeighbors, and SGDClassifier in the first layer and RandomForest in the second layer (output).<br>
Accuracy Achieved: 97.92%
