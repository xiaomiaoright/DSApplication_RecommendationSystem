# DSApplication_RecommendationSystem
# Recommender System
An ML-based recommendation system determines how similar videos or contents or items are to other things you like and then serves up a recommendation. 

## Introduction
**Types of Recommendation system**
- Home page recommendation
- Related item recommendation

**Terminologies**
- Item
- Query (context)
    - User information
    - Addtional context
- Embedding


**Pillars of Recommendation System**
- Candidate generation

- scoring
- re-ranking


### Candidate Generation
- **Two common approaches**
    - Content based filtering
        - Uses similarity between items to recoomend items similar to what the user likes
    - Collaborative filtering
        - Uses similarity between queries and items simultaneously to provide recommendations

- Content based filtering
     - Advantages

        The model doesn't need any data about other users, since the recommendations are specific to this user. This makes it easier to scale to a large number of users.
        The model can capture the specific interests of a user, and can recommend niche items that very few other users are interested in.
    - Disadvantages
        Since the feature representation of the items are hand-engineered to some extent, this technique requires a lot of domain knowledge. Therefore, the model can only be as good as the hand-engineered features.
        The model can only make recommendations based on existing interests of the user. In other words, the model has limited ability to expand on the users' existing interests.

- Collaborative filtering
To address some of the limitations of content-based filtering, collaborative filtering uses similarities between users and items simultaneously to provide recommendations. This allows for serendipitous recommendations; that is, collaborative filtering models can recommend an item to user A based on the interests of a similar user B. Furthermore, the embeddings can be learned automatically, without relying on hand-engineering of features.

    - Example
    When a user visits the homepage, the system should recommend movies based on both:
        - similarity to movies the user has liked in the past
        - movies that similar users liked

     - Choosing Objective Function
        - SGD
        - WALS

    - advantages
        - No domain knowledge necessary
        - Serendipity
        - Great starting point


    - disadvantages
        - Cannot handle fresh items
        - Hard to include side features for query/item
        - 

## About the dataset



## Data Exploration


## Modeling
