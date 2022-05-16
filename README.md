# Recommeder System Approaches

**Data Source**: 
MovieLens 100K rating dataset from [MovieLens](https://grouplens.org/datasets/%20movielens/) (the small dataset recommended for education and development).

:rewind: **1. User-based Collaborative Filtering (UBCF)**:
Implementing user-based collaborative filtering approach by
  - [ ] Using the Pearson correlation function for computing similarities between users.
  - [ ] The prediction function presented in class for predicting movies scores.
  - [ ] Select a user from the dataset, and for this user, show the 10 most similar users and the 20 most relevant movies that the recommender suggests.

:rewind: **2. Item-based Collaborative Filtering (IBCF)**:
Implementing the item-based collaborative filtering approach by, 
  - [ ] Using the cosine similarity for computing similarities between items.
  - [ ] The prediction function presented in class for predicting movies scores.
  - [ ] Select a user from the dataset, and for this user, show the 20 most relevant movies that the recommender suggests.

:rewind: **3. Group Recommendation**:
For producing group recommendation, we will use the user-based collaborative filtering approach as this implemented first. Specifically, for producing group recommendations, we will first compute the movies recommendations for each user in the group, and then we will aggregate the lists of the individual users, so as to produce a single list of movies for the group. We will implement two well established aggregation methods for producing the group recommendations.

   - [ ] Average Aggregation Method:
    The first aggregation approach is the average method. The main idea behind this approach is that all members are considered equals. So, the rating of an item for a group of users will be given be averaging the scores of an item across all group members. 
    Produce a group of 3 users, and for this group, show the top-20 recommendations, i.e., the 20 movies with the highest prediction scores that the average method suggest. 
    
   - [ ] Least Misery Aggregation Method:
    The second aggregation method is the least misery method, where one member can act as a veto for the rest of the group. In this case, the rating of an item for a group of users is computed as the minimum score assigned to that item in all group members recommendations. 
    Produce a group of 3 users, and for this group, show the top-20 recommendations, i.e., the 20 movies with the highest prediction scores that the least misery method suggest. 
   
   - [ ] Recommendation with disagreements:
    Now we will consider disagreements between the users in the group. Here, we will define a way for counting the disagreements between the users in a group, and propose a method that takes disagreements into account when computing suggestions for the group. Use again the group of 3 users, and for this group, show the top-20 recommendations, i.e., the 20 movies with the highest prediction scores that your method suggests. Use the MovieLens 100K rating dataset. 

:rewind: **3. Sequencial Recommendation**:
The goal of the section is to design & implement a new method for producing sequencial group recommendations. Here we are suggesting a simple modifications of the existing approach, e.g., by proposing and using alternatives for group aggregation that ensure good results for the group. Produce a group of 3 users, and for this group, show the top-20 recommenda:ons in 5 different sequences, i.e., the 20 movies with the highest predic:on scores in 5 rounds.


:rewind: **4. why-not questions**: Motivated by the [research paper](https://homepages.tuni.fi/konstantinos.stefanidis/docs/wise20.pdf), the goal is to motivated by the why-not methods for producing explanations for group recommendations for the granularity case for both atomic (e.g., Why not Matrix?) and group (e.g., Why not action movies?) cases, as well as for position absenteeism case (e.g., Why not rank Matrix first?). Producing a group of 3 users, and for this group, show the top-20 recommendations, i.e., the 20 movies with the highest prediction scores, using the MovieLens 100K rating dataset. Given this recommendation list, take as input one why-not question example from each of the above cases and report the corresponding explanations. 










