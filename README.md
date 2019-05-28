# Recommender Systems with Surprise
Project of a recommender system created with the Surprise framework. With a collaborative filtering approach, different algorithms are explored, such as KNN or SVD.

## Python Dependencies
```
  conda install -c conda-forge scikit-surprise 
```

## Examples
<details>
<summary>1. <a href="https://ansegura7.github.io/RS_Surprise/pages/RS_KNN.html" >RS with KNN</a></summary>
<ul>
	<li>Model built from a plain text file</li>
	<li>The algorithm used is: KNNBasic</li>
	<li>Model trained using the technique of cross validation (5 folds)</li>
	<li>The RMSE and MAE metrics were used to estimate the model error</li>
	<li>Type of filtering: user-based collaborative</li>
</ul>
</details>
<details>
<summary>2. <a href="https://ansegura7.github.io/RS_Surprise/pages/RS_SVD.html" >RS with SVD</a></summary>
<ul>
	<li>Model built from a Pandas dataframe</li>
	<li>The algorithm used is: Singular Value Decomposition (SVD)</li>
	<li>Model trained using train and test datasets (80/20)</li>
	<li>The error of the model was estimated using the RMSE metric</li>
	<li>Type of filtering: collaborative</li>
</ul>
</details>
<details>
<summary>3. <a href="https://ansegura7.github.io/RS_Surprise/pages/SR_SVD_Tune.html" >Tune model (SVD)</a></summary>
<ul>
	<li>Model tuning: manual</li>
	<li>Model tuning: automatic</li>
	<li>Compute precision@k and recall@k</li>
</ul>
</details>

## Contributing and Feedback
Any kind of feedback/criticism would be greatly appreciated (algorithm design, documentation, improvement ideas, spelling mistakes, etc...).

## Authors
- Created by Andrés Segura Tinoco
- Created on May 23, 2019

## License
This project is licensed under the terms of the MIT license.

## Acknowledgments
I would like to show my gratitude to:

F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4, Article 19 (December 2015), 19 pages. DOI = http://dx.doi.org/10.1145/2827872
