
Readme
======


Download and save dataset
-------------------------

```
    wget -nc -P ~/scikit_learn_data/mldata/ "https://raw.githubusercontent.com/dmitrii-davidov/Machine-Learning-Data/master/mldata/mnist-original.mat"
```

Load dataset
------------

```
    import sklearn.datasets
    sklearn.datasets.fetch_mldata("MNIST original")
```
