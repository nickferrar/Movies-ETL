# Movies-ETL

# Module 8 Challenge

# Overview:

In this challenge, the purpose is to extract movie data from a Wikipedia JSON file as well as metadata from Kaggle on movies and ratings. The ratings will be uploaded to a 
SQL table and the movie data will be merged from the two sources. 

# Results:

The data was extracted and transformed then loaded onto an SQL database into two tables. The challenge said there would be 6052 movies but my dataset only has 6051. Looking closer
at the data, there was an issue with the movie *The Holiday* where the IMDB link is tt0457939 but from Wikipedia's data it is tt00457939. In the code for this project, 
the wikipedia movies that were extracted had regex string "tt" followed by 7 digits so this movie was not merged into the final DataFrame. 

The ratings table was uploaded as the challenge required. 
