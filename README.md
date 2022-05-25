# Classification-Part-2

This notebook follows on from notebook "Classification Part 1"

In this notebook we will use the well-known Iris dataset to build and analyse the performance of multi-class classifiers. We will first consider a **kNN** classifier and analyse the impact of changing the value of k on the resulting decision regions. We will then train a **logistic regression** classifier and will analyse its performance using the **confusion matrix**. Finally, we will implement a **Bayesian approach** with Gaussian class densities.

# The Dataset

![image](https://user-images.githubusercontent.com/96924468/170327947-7da9fdce-51fc-4cd8-bdfe-110dc11d3f45.png)

Plotting the dataset in the predictor space reveals that the three classes are not linearly separable, i.e. we cannot create straight boundaries in the predictor space that separate samples from different classes.

![image](https://user-images.githubusercontent.com/96924468/170328101-44fa29dd-9b26-45f4-9e7c-b4c943046f0a.png)
![image](https://user-images.githubusercontent.com/96924468/170328120-a4f51db2-d52f-4a97-977d-cbdbfbf8300a.png)
