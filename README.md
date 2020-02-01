# DetectivePikachu
A Network Intrusion Detection System (NIDS) trained on NSL-KDD+ dataset to detect DoS and Probe attacks using different Machine Learning models/algorithms.

## Feature Selection
Feature selection is one of the most important steps. The determination of the proper feature selection algorithm and its use in operations has an effect that will increase the performance of the application. The main problem in feature selection is to select the feature that can best distinguish between classes. Two methods are used here:

#### CfsSubsetEval
The CfsSubsetEval algorithm performs a selection among the attributes in the dataset that those are highly related to the class and that are less important. In this way, the most important features of the dataset are identified. CfsSubsetEval method uses BestFirst search algorithm.

#### Wrapper
The Wrapper algorithm generates multiple subsets from the NSL-KDD+ 20% dataset and uses different classification algorithms (Random Forest, kNN, Gaussian Naive Bayes) to induce classifiers from features in each subset. It then selects the features with the best classifier.

## Requirements
```
sudo apt-get install bro
```

## Reference
Unal Cavusoglu, “A new hybrid approach for intrusion detection using machine learning methods,” http://dx.doi.org/10.1007/s10489-018-01408-x
