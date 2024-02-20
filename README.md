## Movie advisor model

In this project data are split between [movies](https://raw.githubusercontent.com/4GeeksAcademy/k-nearest-neighbors-project-tutorial/main/tmdb_5000_movies.csv") 
and [credits](https://raw.githubusercontent.com/4GeeksAcademy/k-nearest-neighbors-project-tutorial/main/tmdb_5000_credits.csv)

I have downloaded both datasets and added them as 2 different tables of database called 'cine'. I have made a query where i select all columns except duplicates to create a pandas dataframe to work with.
I have processed the columns of this dataframe to create a new column called 'tags' which contains the cast, the director and the synopsis of each film.

Next, I have created a tfidf matrix of the 'tags' value of each film and used cosine distance to know how far is each film from the others.
Then I have used a knn model for the 6 nearest neighbours and trained it with the tfidf matrix.

After this, i have obtained the sorted distances of the 5 nearests neighbours and its indices to build the movie advisor.



