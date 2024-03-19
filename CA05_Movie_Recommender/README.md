# Movie Recommendation System

## Introduction

This project aims to build a recommendation system that suggests movies based on a specific input movie. Utilizing the k-Nearest Neighbors (kNN) algorithm, the system recommends movies by comparing key features such as IMDB ratings, genres (e.g., Biography, Drama, Thriller), and more. For demonstration, this system will recommend 5 movies similar to "The Post" based on predefined criteria.

## Installation

To run this project, you will need Python installed on your machine, along with the following Python libraries:

• pandas
• scikit-learn
• You can install these packages using pip:

>> pip install pandas scikit-learn

## Usage

The main script for the movie recommendation system is recommendation_system.py. To use it, follow these steps:

1. Ensure you have the required libraries installed.
2. Download or clone this repository to your local machine.
3. Run the script in your terminal or command prompt:

>> python recommendation_system.py

This will output the names of 5 movies recommended based on the criteria specified for the movie "The Post".

## How It Works

The recommendation system works by:

1. Loading a dataset of movies with their features from a CSV file.
2. Preparing the dataset by selecting relevant features for comparison.
3. Encoding categorical features to numerical values.
4. Using the k-Nearest Neighbors algorithm to find the closest movies based on the encoded features of "The Post".

## Contributing
Contributions to this project are welcome! Here are a few ways you can help:

1. Report bugs and issues.
2. Suggest improvements or new features.
3. Contribute to the code via pull requests.

## License
This project is open-source and available under the MIT License. See the LICENSE file for more details.
