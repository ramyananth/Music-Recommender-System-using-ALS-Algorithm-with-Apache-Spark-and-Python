For this project, you are to create a recommender system that will recommend new musical artists to a user based on their listening history. Suggesting different songs or musical artists to a user is important to many music streaming services, such as Pandora and Spotify. In addition, this type of recommender system could also be used as a means of suggesting TV shows or movies to a user (e.g., Netflix).

To create this system you will be using Spark and the collaborative filtering technique. The instructions for completing this project will be laid out entirely in this file. You will have to implement any missing code as well as answer any questions.

Datasets

You will be using some publicly available song data from audioscrobbler, which can be found here. However, we modified the original data files so that the code will run in a reasonable time on a single machine. The reduced data files have been suffixed with _small.txt and contains only the information relevant to the top 50 most prolific users (highest artist play counts).

The original data file user_artist_data.txt contained about 141,000 unique users, and 1.6 million unique artists. About 24.2 million users’ plays of artists are recorded, along with their count.

Note that when plays are scribbled, the client application submits the name of the artist being played. This name could be misspelled or nonstandard, and this may only be detected later. For example, "The Smiths", "Smiths, The", and "the smiths" may appear as distinct artist IDs in the data set, even though they clearly refer to the same artist. So, the data set includes artist_alias.txt, which maps artist IDs that are known misspellings or variants to the canonical ID of that artist.

The artist_data.txt file then provides a map from the canonical artist ID to the name of the artist.
