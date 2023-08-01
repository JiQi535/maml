---
layout: default
title: maml.sampling.md
nav_exclude: true
---

# maml.sampling package

Package implementing sampling methods.


## maml.sampling.clustering module

Clustering methods.


### _class_ maml.sampling.clustering.BirchClustering(n: int = 1, threshold_init=0.5, \*\*kwargs)
Bases: `BaseEstimator`, `TransformerMixin`


#### _sklearn_auto_wrap_output_keys(_ = {'transform'_ )

#### fit(X, y=None)

#### transform(PCAfeatures)
## maml.sampling.direct module

## maml.sampling.pca module


### _class_ maml.sampling.pca.PrincipalComponentAnalysis(weighting_PCs=True)
Bases: `BaseEstimator`, `TransformerMixin`

Wrap around PCA in scikit-learn to support weighting PCs.


#### _sklearn_auto_wrap_output_keys(_ = {'transform'_ )

#### fit(normalized_features)

#### transform(normalized_features)
## maml.sampling.stratified_sampling module

Implementation of stratefied sampling approaches.


### _class_ maml.sampling.stratified_sampling.SelectKFromClusters(k: int = 1, allow_duplicate=False)
Bases: `BaseEstimator`, `TransformerMixin`

Wrapper around selection of K data from each cluster.


#### _sklearn_auto_wrap_output_keys(_ = {'transform'_ )

#### fit(X, y=None)
Fit the model.


* **Parameters**


    * **X** – Input features


    * **y** – Target.



#### transform(clustering_data: dict)
Perform clustering.


* **Parameters**

    **clustering_data** – Data to cluster.