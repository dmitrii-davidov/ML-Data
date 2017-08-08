
How to use
==========


SciKit Learn
------------

Fetching:

```
    wget -nc -P ~/scikit_learn_data/mldata/ "https://raw.githubusercontent.com/dmitrii-davidov/Machine-Learning-Data/master/mldata/mnist-original.mat"
```

Loading:

```
    from sklearn.datasets import fetch_mldata
    dataset = fetch_mldata("MNIST original")
```


TensorFlow Examples
-------------------

Fetching:

```
	files=( "t10k-images-idx3-ubyte.gz" "t10k-labels-idx1-ubyte.gz" "train-images-idx3-ubyte.gz" "train-labels-idx1-ubyte.gz" )
	dataset="lecun/mnist"
	for i in ${files[@]}
	do
	    wget -nc -P "~/scikit_learn_data/${dataset}" "https://raw.githubusercontent.com/dmitrii-davidov/Machine-Learning-Data/master/${dataset}/${i}"
	done

```

Loading:

```
	from tensorflow.examples.tutorials import mnist
	dataset = input_data.read_data_sets("~/scikit_learn_data/lecun/mnist", one_hot=True)

```