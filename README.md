# Classification-Part-2

This notebook follows on from notebook "Classification Part 1"

In this notebook we will use the well-known Iris dataset to build and analyse the performance of multi-class classifiers. We will first consider a **kNN** classifier and analyse the impact of changing the value of k on the resulting decision regions. We will then train a **logistic regression** classifier and will analyse its performance using the **confusion matrix**. Finally, we will implement a **Bayesian approach** with Gaussian class densities.

# The Dataset

![image](https://user-images.githubusercontent.com/96924468/170327947-7da9fdce-51fc-4cd8-bdfe-110dc11d3f45.png)

Plotting the dataset in the predictor space reveals that the three classes are not linearly separable, i.e. we cannot create straight boundaries in the predictor space that separate samples from different classes.

![image](https://user-images.githubusercontent.com/96924468/170328101-44fa29dd-9b26-45f4-9e7c-b4c943046f0a.png)
![image](https://user-images.githubusercontent.com/96924468/170328120-a4f51db2-d52f-4a97-977d-cbdbfbf8300a.png)

# kNN Classifiers

The k nearest neighbours (kNN) algorithm is an instance-based method that assigns a new sample to the **majority class** amongst the k closest training samples. From a statistical point of view, we can see kNN as a method that creates **posterior probabilities** by identifying the closest training samples and obtaining the fraction of samples belonging to each class.

The training accuracy for k=1 is 0.94666\
The validation accuracy for k=1 is 0.68
![image](https://user-images.githubusercontent.com/96924468/170328970-5c0d86aa-b58a-48b7-93bf-455a8fe0642f.png)

The training accuracy for k=7 is 0.813333
The validation accuracy for k=7 is 0.77333
![image](https://user-images.githubusercontent.com/96924468/170329175-38f66a98-ce97-43d3-bb30-3314d628706c.png)

The training accuracy for k=13 is 0.8133333
The validation accuracy for k=13 is 0.77333
![image](https://user-images.githubusercontent.com/96924468/170329693-0e42044f-c28b-4d2a-94c9-444ade3d0113.png)

The training accuracy for k=19 is 0.81333
The validation accuracy for k=19 is 0.8
![image](https://user-images.githubusercontent.com/96924468/170329905-36452fab-ad57-45b1-a01a-c1ba35a6b0d4.png)


