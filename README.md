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

The training accuracy for k=1 is 0.94666.
The validation accuracy for k=1 is 0.68

![image](https://user-images.githubusercontent.com/96924468/170328970-5c0d86aa-b58a-48b7-93bf-455a8fe0642f.png)

The training accuracy for k=7 is 0.813333.
The validation accuracy for k=7 is 0.77333
![image](https://user-images.githubusercontent.com/96924468/170329175-38f66a98-ce97-43d3-bb30-3314d628706c.png)

The training accuracy for k=13 is 0.8133333.
The validation accuracy for k=13 is 0.77333
![image](https://user-images.githubusercontent.com/96924468/170329693-0e42044f-c28b-4d2a-94c9-444ade3d0113.png)

The training accuracy for k=19 is 0.81333.
The validation accuracy for k=19 is 0.8
![image](https://user-images.githubusercontent.com/96924468/170329905-36452fab-ad57-45b1-a01a-c1ba35a6b0d4.png)

The training acccuracy for k=25 is 0.826666.
The validation accuracy for k=25 is 0.84
![image](https://user-images.githubusercontent.com/96924468/170330459-156815cb-fbd0-4311-aa50-5a52bd39afe6.png)

The training accuracy for k=31 is 0.8.
The validation accuracy for k=31 is 0.826666
![image](https://user-images.githubusercontent.com/96924468/170330661-a050740d-edb8-432e-8d32-fea4532aca12.png)

The training accuracy for k=37 is 0.786666.
The validation accuracy for k=37 is 0.813333
![image](https://user-images.githubusercontent.com/96924468/170330836-732e4537-a637-4048-a1a9-4e2c96d489c4.png)

The training accuracy for k=43 is 0.73333.
The validation accuracy k=43 is 0.76

![image](https://user-images.githubusercontent.com/96924468/170331020-9188da23-ac3e-474f-874d-71d6eec14470.png)

The training accuracy for k=49 is 0.706666.
The validation accuracy for k=49 

![image](https://user-images.githubusercontent.com/96924468/170331215-be09d5ef-0f79-49d7-ab50-1b2dd0f5fec5.png)

The training accuracy for k=55 is 0.706666.
The validation accuracy for k=55 is 0.7733333
![image](https://user-images.githubusercontent.com/96924468/170331398-caa807b9-fb3e-4c23-9cfc-d4d75225ec79.png)

The training accuracy for k=61 is 0.62666.
The validation accuracy for k=61 is 0.70666
![image](https://user-images.githubusercontent.com/96924468/170331564-718abce4-8c18-480a-915b-6cd9cfae9624.png)

The training accuracy for k=67 is 0.6.
The validation accuracy for k=67 is 0.69333
![image](https://user-images.githubusercontent.com/96924468/170331852-82e45694-282a-459c-b95f-e573b5f76195.png)

The training accuracy for k=73 is 0.493333.
The validation accuracy for k=73 is 0.466666
![image](https://user-images.githubusercontent.com/96924468/170332129-b16bc406-43e0-442b-9646-31444f9c5235.png)

validation accuracy vs k

![image](https://user-images.githubusercontent.com/96924468/170332432-a9b0dd91-ae80-476e-89b3-9b36fe29071c.png)

# Logistic Regression Linear Classifier

The training accuracy of the logistic classifier is 0.8

![image](https://user-images.githubusercontent.com/96924468/170337332-2c2cc55f-482b-4158-80e3-0048179d161a.png)

The validation accuracy of the logistic classifier is 0.82666

![image](https://user-images.githubusercontent.com/96924468/170337505-c9d9b2d4-4cf8-4216-9c8c-8971dcf2bf95.png)

# The Bayesian Perspective

Logistic regression and kNN can be seen as two classification methods that build posterior probabilities and proceed to assign samples to the class with the **highest posterior probability**.

Training accuracy: 0.90909.
Validation accuracy: 0.87272727

![image](https://user-images.githubusercontent.com/96924468/170339163-9349467f-e60c-4e6b-ae0a-3395e3860659.png)

Validation accuracy: 0.76

![image](https://user-images.githubusercontent.com/96924468/170339522-c08fc8f4-1044-494b-a9e7-602a0df8e8de.png)

Validation accuracy: 0.77333

![image](https://user-images.githubusercontent.com/96924468/170339624-edb74323-8c86-4bfd-84d7-e96a8cfc8b84.png)


