# Paican


Tensorflow implementation of the method proposed in the paper: "Bayesian Robust Attributed Graph Clustering: Joint Learning of Partial Anomalies and Group Structure", Aleksandar Bojchevski and Stephan Günnemann, AAAI 2018.

## Installation
```bash
python setup.py install
```

## Requirements
* tensorflow (>=1.4)
1* sklearn (only for evaluation)

## Data
Each of the dataset folders consists of the following files:

* A.mtx - the adjacency matrix in scipy's sparse csr_matrix format
* X.mtx - the attribute matrix in scipy's sparse csr_matrix format
* feature_to_index.npy - a dictionary mapping a feature label to index (e.g. 'neurology' -> 5)
* node_to_index.npy - a dictionary mapping a node label (e.g name of a person or paper ID) to index
* z.npy - ground truth clusters if available
* label_to_cluster.npy - a dictionary mapping a label (e.g. journal, party) to cluster index

## Demo
See the notebook example.ipynb for a simple demo.

## Cite
Please cite our paper if you use this code in your own work.
