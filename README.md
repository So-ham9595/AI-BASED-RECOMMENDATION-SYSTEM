# AI-BASED-RECOMMENDATION-SYSTEM

COMPANY: CODETECH IT SOLUTIONS

NAME: Soham Santosh Salunkhe

Intern ID :CITS0D507

DOMAIN: JAVA PROGRAMMING

BATCH DURATION: 4 Weeks from June 17th 2025 to July 14th 2025.

MENTOR NAME: NEELA SANTHOSH

The RecommendationApp is a Java-based recommendation system built using the Apache Mahout machine learning library. It implements a user-based collaborative filtering algorithm to provide personalized item recommendations based on user preferences. This project is a powerful example of how to use Mahout to process user-item rating data and generate recommendations using similarity measures and neighborhood models.

At its core, the application loads user ratings from a CSV file named ratings.csv located in a data directory. The file must follow Mahout’s standard format, where each line typically represents a user ID, item ID, and rating (e.g., 1,101,4.5). The ratings are parsed and stored using Mahout's FileDataModel class, which creates a structured DataModel representing all user-item interactions. This model serves as the foundation for all subsequent computations.

To determine how similar users are to each other, the program uses Pearson Correlation Similarity via the PearsonCorrelationSimilarity class. This statistical method calculates the degree of linear correlation between two users' rating patterns, which helps in identifying users with similar preferences. Once similarity scores are computed, the application uses the NearestNUserNeighborhood class to find the two most similar users (neighbors) to a target user. This neighborhood-based approach ensures that recommendations are generated by focusing only on those users who are most alike.

The recommender is then constructed using GenericUserBasedRecommender, which takes the data model, user similarity, and neighborhood as input. The recommendation engine applies user-based collaborative filtering by analyzing the preferences of similar users to suggest items that the target user has not yet rated but is likely to enjoy. In this specific case, the system generates three recommendations for user ID 1 using the recommend(1, 3) method call.

When the application is executed, it prints a list of recommended items for user 1. Each recommendation includes an item ID and an estimated preference score, which indicates how strongly the system believes the user will like the item. The higher the score, the better the match.

In the screenshot provided, the application is compiled and run using external Mahout libraries (included via the -cp ".;lib/*" command), confirming successful integration of third-party libraries. The terminal shows the system executed successfully and began outputting recommendations for the user, although no items are listed in this example (likely due to missing or incomplete ratings.csv data or no strong matches found).

This project is highly beneficial for understanding collaborative filtering, a widely used technique in real-world recommendation systems like those used by Netflix, Amazon, or Spotify. It introduces key concepts such as user similarity, neighborhood models, recommendation engines, and preference estimation.

Overall, this Java application provides a clean, practical implementation of a user-based recommender system using Apache Mahout. It’s a strong starting point for anyone interested in building personalized recommendation engines and can be extended with additional features like item-based filtering, hybrid methods, GUI integration, or real-time recommendations via a web interface.

# OUTPUT
![Image](https://github.com/user-attachments/assets/fd82a4c3-410e-4cce-a4b1-67ffbf60f06f)
