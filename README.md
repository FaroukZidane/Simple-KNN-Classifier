# Simple Animal Classifier using k-Nearest-Neighbor Algorithm

------



## Introduction

The k-Nearest Neighbor classifier is by far the most simple machine learning and image classification algorithm. In fact, it’s so simple that it doesn’t actually “learn” anything. Instead, this algorithm directly relies on the distance between feature vectors (which in our case, are the raw RGB pixel intensities of the images). The distance used here is the Euclidean distance:

![](https://github.com/FaroukZidane/Simple-KNN-Classifier/raw/master/doc/images/knn-l2-dist.png)

In this project, we will use KNN algorithm to classify between images of dogs, cats and pandas.

<img src="https://github.com/FaroukZidane/Simple-KNN-Classifier/raw/master/doc/images/knn.png" style="zoom:50%;" />

------

## Pre-requisites

- Python 3.6.9
- scikit-learn 0.22.2
- imutils
- argparse

*NOTE: The versions of the modules mentioned above are the exact versions used in this project. Please confirm if it works with different versions with you. Also, you may find one ort more of these packages already installed in your system or pre-installed with python*



## The Dataset

The “Animals” dataset is a simple example dataset to demonstrate how to train image classifiers using simple machine learning techniques as well as advanced deep learning algorithms. Images inside the Animals dataset belong to three distinct classes: dogs, cats, and pandas, with 1,000 example images per class.

![](https://github.com/FaroukZidane/Simple-KNN-Classifier/blob/master/doc/images/dataset.png?raw=true)



Dataset kaggle link: [HERE](https://www.kaggle.com/ashishsaxena2209/animal-image-datasetdog-cat-and-panda/data)

------



## Training

Download the dataset from the link above. Then simply, execute the following terminal command in the project repository. 

```
$ python knn.py --dataset PATH_TO_DIR/datasets/animals
```

*Remove `PATH_TO_DIR` and add your own path of the animal dataset folder.*



------



## KNN Results

- **K = 1**



```
              precision    recall  f1-score   support

        cats       0.41      0.48      0.44       249
        dogs       0.42      0.55      0.47       262
       panda       0.79      0.37      0.51       239
    
    accuracy                           0.47       750

   macro avg       0.54      0.47      0.47       750
weighted avg       0.53      0.47      0.47       750
```

- **K = 2**

```
              precision    recall  f1-score   support

        cats       0.39      0.69      0.50       249
        dogs       0.38      0.37      0.38       262
       panda       0.92      0.20      0.33       239

    accuracy                           0.43       750
   macro avg       0.57      0.42      0.40       750
weighted avg       0.56      0.43      0.40       750


```

