# movielens-recommender

Part of a final project for a graduate course in Data Analytics at the University of Toronto (Winter term, 2016). Our group set out to create a movie recommendation engine that would recommend movies that would have a high chance of being enjoyed by the user.

## Background

This was a final project for a graduate course offered in the Winter Term (January-April, 2016) at the University of Toronto, Faculty of Information: INF2190 Data Analytics: Introduction, Methods, and Practical Approaches. Our group's full tech stack for this project was expressed in the acronym *MIPAW*: MySQL, IBM SPSS Modeler, Python, AWS, and Weka.

Running the model on a sample of the MovieLens movie ratings data produced movie recommendations where >85% would produce favorable ratings.

## Datasets

The following main data sources were used for this project.

- [MovieLens](http://grouplens.org/datasets/movielens/)
- [MovieLens Tag Genome](http://grouplens.org/datasets/movielens/tag-genome/)
- [IMDb](http://www.imdb.com/interfaces)

### MovieLens 

The MovieLens movie ratings data is provided by GroupLens Research in datasets ranging in size from 100K to 20 million. There is a "Latest" dataset that includes more recent ratings data up to 2016. Our team chose to use the stable 20 million (MovieLens 20M) count dataset and the Latest dataset.

Permalink (20M): http://grouplens.org/datasets/movielens/20m/

Permalink (Latest): http://grouplens.org/datasets/movielens/latest/

### MovieLens Tag Genome

Tag Genome data is also from GroupLens Research. In this dataset, the relevance of certain tags to a range of movies was calculated using a machine learning algorithm by the research team.

Permalink: http://grouplens.org/datasets/movielens/tag-genome/

### IMDb

The IMDb plain text data dumps are available through 2 FTP sites. 

Permalink: http://www.imdb.com/interfaces


## Recommendation System

### Tech Stack

Each part of the tech stack used for this project was used to different degrees by each team member. 

- MySQL - primary database
- IBM SPPS Modeler - analytics software for generating models
- Python - data pre-processing and data analytics implementation
- Amazon Web Services - cloud computing in conjunction with MySQL
- Weka - data mining tool

### Technique

I undertook my share of the project with inspiration from the [Collaborative Filtering](https://en.wikipedia.org/wiki/Collaborative_filtering) technique, which takes advantage of the predictive power of analyzing like-minded users. For example, if each tuple is structured as [id, movieId, rating], then the tuples [246, 2, 3.5] and [357, 2, 3.5] would suggest that both users 246 and 357 are like-minded in that they rated movie "2" with a "3.5" rating. This underlying technique was combined with further processing steps and implemented in a Python CLI tool.

## Next Steps



