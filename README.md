<br/>
<p align="center">
  <a href="https://github.com/Srijansarkar17/MovieRecommendationSystem">
    <img src="https://editor.analyticsvidhya.com/uploads/76889recommender-system-for-movie-recommendation.jpg" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">MovieRecommendationSystem</h3>

  <p align="center">
    Recommends you movies according to your taste
    <br/>
    <br/>
    <a href="https://github.com/Srijansarkar17/MovieRecommendationSystem"><strong>Explore the docs »</strong></a>
    <br/>
    <br/>
    <a href="https://github.com/Srijansarkar17/MovieRecommendationSystem">View Demo</a>
    .
    <a href="https://github.com/Srijansarkar17/MovieRecommendationSystem/issues">Report Bug</a>
    .
    <a href="https://github.com/Srijansarkar17/MovieRecommendationSystem/issues">Request Feature</a>
  </p>
</p>

![Downloads](https://img.shields.io/github/downloads/Srijansarkar17/MovieRecommendationSystem/total) ![Contributors](https://img.shields.io/github/contributors/Srijansarkar17/MovieRecommendationSystem?color=dark-green) ![Forks](https://img.shields.io/github/forks/Srijansarkar17/MovieRecommendationSystem?style=social) ![Stargazers](https://img.shields.io/github/stars/Srijansarkar17/MovieRecommendationSystem?style=social) ![Issues](https://img.shields.io/github/issues/Srijansarkar17/MovieRecommendationSystem) 

## Table Of Contents

* [About the Project](#about-the-project)
* [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
* [Usage](#usage)
* [Contributing](#contributing)
* [Authors](#authors)

## About The Project

This project recommends five movies to the user according to his search of the movie.

Dataset:
The dataset for this movie is divided into two parts and it is taken from Kaggle which is sourced from Tmdb and it gives information about 5000 movies. 

Data Preprocessing:
First of all I started with basic Data Preprocessing Techniques like removing the null values and removing duplicates. Then the project gets complex as we will deal with textual columns in this dataset rather than numerical columns. Then we select the features that is needed to train the model and remove the rest.

Text Preprocessing:
Then we apply the NLTK library to do some basic text preprocessing like removing the stop words and we also applied stemming. We preprocessed the textual columns as the data contained a lot of information which was not needed. We only needed the genre name from the genres column and only needed the necessary values from the keywords, crew and cast column respectively. We combined all the important values from all those columns and combined it into a single column called Tags.

Vectorization of Text in the Tag Column:
We needed to convert the textual column of Tag into Vectors so that cosine similarity can be applied to it. We converted it into vectors on the basis of most common 5000 words so the shape of the vectorized text came out to be (4806,5000).

Applying Cosine Similarity for building the Recommendation System:
Cosine similarity is a measure used in machine learning and natural language processing to determine the similarity between two vectors in a high-dimensional space. It calculates the cosine of the angle between the vectors, which indicates how closely related they are in terms of direction, regardless of their magnitude. The text that was converted into vectors have some angle between them and that angle decides the similarity between each and every vector i.e movie.


## Built With



* [Python](https://www.python.org/)
* [Pandas](https://pandas.pydata.org/)
* [Numpy](https://numpy.org/)
* [Scikit-Learn](https://scikit-learn.org/stable/)
* [NTLK](https://www.nltk.org/)

## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

You can download Anaconda and use their Jupyter Notebook
https://www.anaconda.com/download
You have to install these datasets so that you can work on them:
Dataset Links: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

## Usage

A movie recommendation system employs algorithms to analyze user data, offering personalized suggestions based on viewing history and preferences. By considering factors like genre and ratings, it efficiently predicts movies users are likely to enjoy, enhancing their experience. Furthermore, it promotes undiscovered content, broadening users' cinematic horizons. These systems drive user engagement and retention for streaming platforms by delivering tailored recommendations, fostering satisfaction and loyalty. In summary, movie recommendation systems optimize content discovery, enrich user experience, and contribute to the success of the entertainment industry.

_For more examples, please refer to the [Documentation](https://example.com)_

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/Srijansarkar17/MovieRecommendationSystem/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
* Please make sure you check your spelling and grammar.
* Create individual PR for each suggestion.
* Please also read through the [Code Of Conduct](https://github.com/Srijansarkar17/MovieRecommendationSystem/blob/main/CODE_OF_CONDUCT.md) before posting your first idea as well.

### Creating A Pull Request

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Authors

* **Srijan Sarkar** - *Comp Sci Student* - [Srijan Sarkar](https://github.com/Srijansarkar17) - *Built the whole Project*


