### Readme for Failed - Movie Recommendation System Project

#### Project Overview
This project aimed to develop a movie recommendation system based on movie descriptions. The dataset includes over 700,000 movies, with features like title, genres, overview, and more. We initially attempted to use Word2Vec for generating semantic embeddings of movie descriptions. However, due to the dataset's large size and the high computational demands of Word2Vec, we faced significant challenges.

#### Challenges Encountered
1. **Computational Limitations with Word2Vec**: 
   - The first major challenge was the computational demand of processing such a large dataset with Word2Vec. Even with Google Colab's resources, the task was not feasible. This was partly due to the memory and processing power needed to generate word embeddings for over 700,000 movie descriptions.
   
2. **Switch to Google Colab Pro**: 
   - To address this, we upgraded to Google Colab Pro for more computational power. Despite this upgrade, the system continued to face difficulties in handling the dataset's size without crashing.

3. **Attempt to Store and Reuse Embeddings**: 
   - We then attempted a strategy to process the embeddings, store them in a file, and download them for later use. However, this approach also led to crashes, likely due to the sheer size of the data and the limitations of the platform's memory.

#### Adjustments and Simplification
To manage these challenges, we made several adjustments:
1. **Switch to GloVe Embeddings**: 
   - We switched from Word2Vec to GloVe (Global Vectors for Word Representation). GloVe provides pre-trained word embeddings that are generally smaller and less computationally intensive to load and use.
   
2. **Dimensionality Reduction with PCA**: 
   - We applied PCA (Principal Component Analysis) to reduce the dimensionality of our embeddings, thereby lessening the computational load.

3. **Focusing on a Subset of Data**: 
   - As a further measure, we reduced the scope of our dataset by focusing on the top 10% of movies based on `vote_average`. This reduction in data size helped to make the computation more manageable.

#### Purpose of Using Word2Vec/GloVe
The rationale behind using Word2Vec (and later GloVe) was to capture the semantic meaning of movie descriptions. These models translate text into numerical vectors, considering the context and semantic relationships between words. This way, movies with semantically similar descriptions are identified as similar, allowing for more nuanced recommendations than simple keyword matching.

#### Conclusion
In this project, we learned a crucial lesson about the limits of handling very large datasets, especially when using complex tools like Word2Vec and GloVe. Even with extra computing power from Google Colab Pro, dealing with over 700,000 movie descriptions was just too much. This challenge made us switch to a smaller dataset and try different methods. It showed us how important it is to match our project goals with what's actually possible given our available resources.
