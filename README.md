# Movie Recommendation System
A movie recommendation system, also referred to as a Movie Recommender System, leverages machine learning techniques to anticipate or filter users' film preferences by analyzing their past choices and behaviors.

Typically, these systems consist of two primary components: users and items (movies in this context). The primary objective is to accurately filter and predict the movies that a user is most inclined to watch, thereby enhancing their viewing experience.

Among the diverse filters available, one commonly adopted approach is Content-based Filtering. This method assesses the intrinsic qualities and characteristics of movies, such as genre, plot keywords, actors, directors, and more, to recommend films that align closely with the user's demonstrated preferences and interests. By focusing on the content attributes of movies and comparing them with the user's historical interactions, content-based filtering can offer personalized and relevant movie suggestions.

![image](https://github.com/abhixxhek/Movie-Recommendation-System/assets/93929650/2713053a-a4d2-4e10-8b29-daf449c2657b)

# Working of the Model

1. Create a DataFrame: Construct a DataFrame comprising movie title, movie ID, and tags. Tags encompass various relevant items like cast, crew, genre, description, and keywords associated with each movie.
2. Handling Missing Values and Duplicates: Eliminate any null values and duplicate entries from the tags section to ensure data quality and accuracy.
3. Stemming: Apply stemming to the tags column to reduce each word to its root form, facilitating semantic similarity analysis.
4. Vectorization: Utilize CountVectorizer to transform the tags section into a matrix of token counts, representing the frequency of each word in the corpus.
5. Cosine Similarity: Compute cosine similarity between the vectorized representations of different movies, measuring the cosine of the angle between their feature vectors.
6. Identifying Similar Movies: Determine the top 5 most similar movies for each movie based on cosine similarity scores.
7. Interactive Retrieval: Present the recommended movie titles in a user-friendly format, allowing easy interpretation and exploration. This could be in bullet points or a formatted list, enhancing readability and engagement.
