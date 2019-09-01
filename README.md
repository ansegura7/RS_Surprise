# Recommender Systems with Surprise
Project with examples of different recommendation system created with the <a href='http://surpriselib.com/' target='_blank'>Surprise</a> framework. With a collaborative filtering approach, different algorithms are explored, such as KNN or SVD.

## Examples
<details open>
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
<summary>3. <a href="https://ansegura7.github.io/RS_Surprise/pages/RS_SVD_Tune.html" >Tune model (SVD)</a></summary>
<ul>
	<li>Model tuning: manual</li>
	<li>Model tuning: automatic</li>
	<li>Compute precision@k and recall@k</li>
</ul>
</details>

## Data
MovieLens data sets were collected by the GroupLens Research Project at the University of Minnesota.
 
This data set consists of:
- 100,000 ratings (1-5) from 943 users on 1682 movies. 
- Each user has rated at least 20 movies. 
- Simple demographic info for the users (age, gender, occupation, zip)

Table format: **u.data**

| user id | item id | rating | timestamp |
| -- | -- | -- | -- |
| 196 | 242 | 3 | 881250949 |
| 186 | 302 | 3 | 891717742 |
| 22 | 377 | 1 | 878887116 |
| 244 | 51 | 2 | 880606923 |
| 166 | 346 | 1 | 886397596 |

Table format: **u.item**

| movie id | movie title | release date | IMDb URL |
| -- | -- | -- | -- |
| 1 | Toy Story (1995) | 01-Jan-1995 | http://us.imdb.com/M/title-exact?Toy%20Story%20(1995) |
| 2 | GoldenEye (1995) | 01-Jan-1995 | http://us.imdb.com/M/title-exact?GoldenEye%20(1995) |
| 3 | Four Rooms (1995) | 01-Jan-1995 | http://us.imdb.com/M/title-exact?Four%20Rooms%20(1995) |
| 4 | Get Shorty (1995) | 01-Jan-1995 | http://us.imdb.com/M/title-exact?Get%20Shorty%20(1995) |
| 5 | Copycat (1995) | 01-Jan-1995 | http://us.imdb.com/M/title-exact?Copycat%20(1995) |

Table format: **u.user**

| user id | age | gender | occupation | zip code |
| -- | -- | -- | -- | -- |
| 1 | 24 | M | technician | 85711 |
| 2 | 53 | F | other | 94043 |
| 3 | 23 | M | writer | 32067 |
| 4 | 24 | M | technician | 43537 |
| 5 | 33 | F | other | 15213 |

<a href="https://grouplens.org/datasets/movielens/100k/" target="_blank">Permalink</a>

## Python Dependencies
``` console
  conda install -c conda-forge scikit-surprise 
```

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
