"# choose-lenses-ANN-SVM-" 

 
1- Description of the problem
For types of contact lenses, different patients have a different selection method, when there is a large factor in the patient's eye monitoring data types, the need to take them into account will be more numerous and complex, in this case, there may not be many experienced clinicians and this It gives a good fit for the types of contact lenses that the patient wears. In this case, if the patient's eye contains a large number of known types of contact lenses and obsolete monitoring data, it can be replaced doctor by the data of the SVM   and ANN and KNNfor  determine the type of contact lens of the patient.

2. Data preparation and Load data
Contact dataset for text documents "lenses.txt" where each row is indicated by the patient's condition and the type of contact lens-wearing eye condition. The first column is the patient's age, followed by each column the patient's type of astigmatism whether the last column is the type of lens the patient wears.
3- Data understanding,Data Visualization, featureselection andStandardization: -
Looking at the lenses.cvs file, we see that the data has 24 number of instances with 4 attributes:
•	age of the patient [ young, pre-presbyopic, prespyopic]
•	spectacle prescription [ myope, hypermetrope]
•	astigmatic: [no, yes]
•	tear production rate: [reduced, normal]
4- label classes:
•	hard contact lenses
•	soft contact lenses
•	no contact lenses
 
5- Splitting dataset
The next step is splitting the dataset. We saw already above how to measure the amount of disorder in the dataset. Here, we measure the entropy, split the dataset, measure the entropy on the split sets, and see if splitting it was the right thing to do. We will do this for all of our features to determine the best feature to split on.

6- Modelling
3.1. ANN (Artificial Neural Network)
Artificial neural networks are one of the main tools used in machine learning. As the “neural” part of their name suggests, they are brain-inspired systems which are intended to replicate the way that we humans learn.
3.2. KNN (K-Nearest Neighbors)
In Supervised Learning, KNN are one of the most popular and most used machine learning algorithms. Some libraries like scikit-learn implements this algorithm which facilitates their usage. However, in this project.
3.3. SVM (Support Vector Machine)
Support Vector Machines (SVM for short) are supervised machine learning algorithms used for classification and regression purposes. In this kernel, I built a Support Vector Machines classifier to classify fitting contact lenses. I used a contact lens dataset to predict this project.








ANN (Artificial Neural Network):-
Neural networks consist of input and output layers, as well as (in most cases) a hidden layer consisting of units that transform the input into something that the output layer can use. ANNs have three layers that are interconnected. The first layer consists of input neurons. Those neurons send data on to the second layer, which in turn sends the output neurons to the third layer. ANNs are considered non-linear statistical data modeling tools where the complex relationships between inputs and outputs are modeled or patterns are found. Note that a neuron can also be referred to as a perceptron.
Steps
1-	Weights Initialization
2-	Inputs Application
3-	Sum of input weight products
4-	Activation function response calculation 
5-	Weights Adaptation 
6-	Back to step 2
 
KNN (K-Nearest Neighbors): -
K-Nearest Neighbor classifier is one of the introductory supervised classifiers, which every data science learner should be aware of. This algorithm was first used for a pattern classification task which was first used by Fix & Hodges in 1951. To be similar the name was given as KNN classifier. KNN aims for pattern recognition tasks. 
K-Nearest Neighbor also known as KNN is a supervised learning algorithm that can be used for regression as well as classification problems. Generally it is used for classification problems in machine learning. 

KNN algorithm pseudo code implementation
1.	Load the desired data. 
2.	Choose the value of k.
3.	For getting the class which is to be predicted, repeat starting from 1 to the total number of training points we have.
4.	The next step is to calculate the distance between the data point whose class is to be predicted and all the training data points. Euclidean distance can be used here.
5.	Arrange the distances in non-decreasing order. 
6.	Assume the positive value of k and filtering k lowest values from the sorted list.
7.	We have top k top distances.
8.	Let ka represent the points that belong to the ath class among k points.
9.	If ka>kb then put x in the class.

 
Support Vector Machines
Support Vector Machine (SVM) is a supervised machine learning algorithm which can be used for both classification or regression challenges. However, it is mostly used in classification problems. In the SVM algorithm, we plot each data item as a point in n-dimensional space (where n is number of features you have) with the value of each feature being the value of a particular coordinate. Then, we perform classification by finding the hyper-plane that differentiates the two classes very well (look at the below snapshot).

2. Support Vector Machines intuition 
Now, we should be familiar with some SVM terminology.
Hyperplane
A hyperplane is a decision boundary which separates between given set of data points having different class labels. The SVM classifier separates data points using a hyperplane with the maximum amount of margin. This hyperplane is known as the maximum margin hyperplane and the linear classifier it defines is known as the maximum margin classifier.
Support Vectors
Support vectors are the sample data points, which are closest to the hyperplane. These data points will define the separating line or hyperplane better by calculating margins.
Margin
A margin is a separation gap between the two lines on the closest data points. It is calculated as the perpendicular distance from the line to support vectors or closest data points. In SVMs, we try to maximize this separation gap so that we get maximum margin.
 


