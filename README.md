
SWKM
====

The goal of SWKM is to perform (Sparse) Weighted K-Means algorithm on observations with weights. If some observations are known to be noisier than the others, the method in this package can be applied to adaptively tune weights and cluster the data.

Installation
------------

You can install the released version of SWKM from Github:

``` r
devtools::install_github("cuhklinlab/SWKM")
```

As this package depends on the RcppArmadillo package, Windows users should install [Rtools](https://cran.r-project.org/bin/windows/Rtools/) in advance to compile the package.

Main Functions
--------------

`kmeans.weight`: Perform weighted K-Means algorithm on data.

`kmeans.weight.tune`: Choose weight parameter for (sparse) weighted K-Means algorithm. Usually used before `kmeans.weight` or `KMeansSparseCluster.weight`.

`KMeansSparseCluster.weight`: Perform sparse weighted K-Means algorithm on data.

`KMeansSparseCluster.permute.weight`: Choose sparsity parameter for sparse weighted K-Means algorithm. Usually used before `KMeansSparseCluster.weight`, and after weight parameter is tuned or known.

`ChooseK`: Choose the number of clusters K for (sparse) weighted K-Means clustering. Usually used before clustering method is performed.

Examples
--------

Please refer to the [vigenette](https://github.com/cuhklinlab/SWKM/tree/master/doc) with two examples for a quick guide to SWKM package.
