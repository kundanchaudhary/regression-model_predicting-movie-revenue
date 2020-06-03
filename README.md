# Predicting Revenue Of Pre-Released Movies

## Description:
Film production is a huge financial risk. Currently, blockbuster movies can have budgets in excess of hundreds of millions of dollars. This risk could be reduced to an extent with the use of quantitative modeling. 

## Objective:
Since movie scripts are pitched and budgets are set and spent well before any revenue is ever made, we plan to construct a predictive model using features that are generally known before the movie release date such as the movie length, budget, and genre.

## Methodology:
We used IMDB (https://www.imdb.com/search/title/?title_type=feature&release_date=1972-01-01,2020-01-10&count=250) to acquire various information related to a given movie released between 1972 to 2020. We used Beautiful Soup to scrape data (movie titles, released year, ratings, metascore, votes by IMDB users, length, genre, and so on) from each page. We cleaned and scaled the relevant features using pandas library. Linear and polynomial regression with regularization (ridge and lasso) were performed. We chose the model with the least mean squared error and the largest adjusted r-squared value to test on our test dataset.

## Results/Conclusions:
In this project, we find that ridge regression performs the best in terms of predicting target variable with the features we used. Budget plays a dominant role in predicting the worldwide gross of a movie. Additionally, our model indicates that adventure, animation, thriller category movies would produce more worldwide gross in comparison to some genres such as war, history, or fantasy. Furthermore, the model can be improved by taking more data points representing higher worldwide gross (>$500,000,000), and adding more features such as the inclusion of certain actors or directors in the movie which have higher popularity (say, in terms of awards).

## References:

[1] Aurelien Geron, _Hands-On Machine Learning with Scikit-Learn & TensorFlow_, 2017.

[2] Andreas Muller & Sarah Guido, _Introduction to Machine Learning with Python_, 2017.