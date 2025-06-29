# Movie-Recommendation-System  🎬

This is a simple content-based movie recommendation system I built using Python and pandas. It suggests similar movies based on the one you input by comparing genres, cast, crew, and keywords.

### What’s inside

- Jupyter notebook with the code and explanation
- Datasets: `movies_metadata.csv` and `links_small.csv`

## How it works

-There are Various Modes of Recommendation System
### 1. Weighted Average Recommendation (Simple)
    This method uses two key numeric features:
    - `vote_average` (how well-rated a movie is)
    - `vote_count` (how many people rated it)
A weighted Score is calculated to recommend movies that are both popular and highly rated
Formula Used:


**(v / (v + m)) * R + (m / (v + m)) * C**

  Where :
  - `V` = vote count
  -  `R` = vote average
  -  `C` = mean vote across all movies
  -  `m` =  min. votes required to be listed
### 2. Content-Based Recommendation (Cosine Similarity)
 Uses metadata like:
 - Movie Overview (Plot Summary)
 - Tags or keywords
 - Genres

These textual features are vectorized using **TF-IDF** and then similarity is calculated using **cosine similarity** Movies with similar description are recommended based on input title

### 3.Advanced Collaborative Filtering

More complex Techniques like **matrix factorization**, **neural networks** can be used to Design a great Movie Recommendation System.


#### The Content-Based Recommendation system worked like this:
- It uses TF-IDF and cosine similarity to figure out which movies are most similar based on the metadata.
- Just enter a movie name, and it’ll show you some that are similar.

## Example:  
Input: The Dark Knight


Output: Batman Begins, The Prestige, Inception, etc.


## Tech used

- Python
- pandas
- scikit-learn
- Jupyter Notebook

 ## Made by

[@Kartaverya](https://github.com/Kartaverya)
