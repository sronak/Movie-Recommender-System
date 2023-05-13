# Movie Recommendation System

This project implements a movie recommendation system using collaborative filtering, content-based filtering, and popularity-based recommendations. It utilizes the MovieLens dataset for movies and ratings.

## Table of Contents

- [Introduction](#introduction)
- [Data Exploration](#data-exploration)
- [Popularity-Based Recommendations](#popularity-based-recommendations)
- [Content-Based Recommendations](#content-based-recommendations)
- [Collaborative Filtering](#collaborative-filtering)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The movie recommendation system is designed to suggest movies to users based on different approaches. It includes three main recommendation techniques:

1. Popularity-based recommendations: This approach suggests popular movies based on average ratings and the number of ratings.
2. Content-based recommendations: This approach suggests movies similar to the user's preferred genres using TF-IDF vectorization.
3. Collaborative filtering: This approach suggests movies based on the preferences of similar users.

The code provided demonstrates the implementation of these techniques using the MovieLens dataset.

## Data Exploration

The initial step involves understanding the dataset by performing exploratory data analysis (EDA). The code explores the movies and ratings datasets, checks for missing values, analyzes the distribution of ratings, and identifies unique users and movies.

## Popularity-Based Recommendations

The popularity-based recommendations are based on the average ratings and the number of ratings for each movie. The code provides a user-defined function to fetch top N popular movies for a given genre and minimum number of ratings.

## Content-Based Recommendations

The content-based recommendations focus on movie genres. The code uses TF-IDF vectorization to convert movie genres into numerical vectors. It then calculates cosine similarity to find movies with similar genres. A user-defined function is provided to generate recommendations based on genre similarity.

## Collaborative Filtering

Collaborative filtering recommends movies based on the preferences of similar users. The code includes a function to generate recommendations for a target user. It finds similar users based on their movie ratings and suggests movies that the target user has not watched.

## Usage

To use this movie recommendation system, follow these steps:

1. Clone the repository: `git clone https://github.com/sronak/movie-recommendation-system.git`
2. Install the required dependencies (see Dependencies section).
3. Prepare the movie and ratings datasets in CSV format.
4. Update the file paths in the code to point to the correct dataset files.
5. Run the code and explore the different recommendation techniques.

## Dependencies

The following libraries are required to run the code:

- pandas
- numpy
- scikit-learn
- matplotlib
- wordcloud
- ipywidgets

You can install them using pip:
pip install pandas numpy scikit-learn matplotlib wordcloud ipywidgets

## Contributing

Contributions to this movie recommendation system are welcome. Feel free to open issues or submit pull requests with improvements or new features.

## License

This project is licensed under the [MIT License](LICENSE).
