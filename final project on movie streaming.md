1.INTRODUCTION:

I wondered, how the movie streaming platform could suggest me content that appealed to me. Then I came across something known as Recommendation System. 
This system is capable of learning my watching patterns and providing me with relevant suggestions.
 Having witnessed the fourth industrial revolution where Artificial Intelligence and other technologies are dominating the market, I am sure that you must have come across a recommendation system in your everyday life. I am also sure that by this time curiosity must be getting the best of you.
  1.1  Goal of the project:
 
 The main goal of this machine learning project is to build a recommendation engine that recommends movies to users and also to understand how exactly it works.

2.DATA:

A recommendation system provides suggestions to the users through a filtering process that is based on user preferences and browsing history.

  2.1The information about the user is taken as an input. 
  
  2.2The information is taken from the input that is in the form of browsing data. 

This information reflects the prior usage of the product as well as the assigned ratings.
A recommendation system is a platform that provides its users with various contents based on their preferences and likings. A recommendation system takes the information about the user as an input. The recommendation system is an implementation of the machine learning algorithms.
A recommendation system also finds a similarity between the different products.
 For example, Netflix Recommendation System provides you with the recommendations of the movies that are similar to the ones that have been watched in the past. 
Furthermore, there is a collaborative content filtering that provides you with the recommendations in respect with the other users who might have a similar viewing history or preferences. 

3.DATASET AND REFERENCES:

In order to build our recommendation system, we have used the MovieLens Dataset.  This data consists of 105339 ratings applied over 10329 movies.


4.Importing Essential Libraries

In our Data Science project, we will make use of these four packages – ‘recommenderlab’, ‘ggplot2’, ‘data.table’ and ‘reshape2’.

5.METHODOLOGY:

  5.1Collaborative filtering
  
The idea of a collaborative filtering approach is to collect and analyze a large amount of information about user actions and settings and then predict which users will favor their similarity with other users .
The advantage of collaborative filtering is that it does not rely on content that can be analyzed and can accurately represent complex items. 
Algorithms are used to calculate user similarities or item similarities in recommender systems, such as k-nearest neighbors and Pearson correlation. 
Another collaborative filtering concept is based on assumptions. People who buy in the past will buy in the future and like the same product them like in the past.

When modeling from user actions, differences often occur between actual and predicted data collection models. One of the most popular examples of collaborative filtering is item-to-item collaborative filtering (Users who bought A also buy B). The Weaknesses of collaborative filtering methods include cold start, scalability, and sparsity. There are two types of collaborative filtering methods: memory-based and model-based collaborative filtering.

  5.2k-cliques detection in social network
  
     The k-clique is a complete graph which has k nodes. In complex networks, there are usually a lot of complete graphs which have different scales. Generally, the value of k is      greater than or equal to at least 3. If k is equal to 2, this means that. There is only an edge, which has little practical meaning.

  5.3Cosine similarity measure
  
     Cosine similarity is a similarity function that is often used in information retrieval, and it is also one of the most popular similarity calculations applied to text       documents, for numerous information retrieval applications , as well as clustering .
     When documents are represented as vectors, the similarity in two documents corresponds to the correlation between the vectors. This is quantified as the cosine of the angle between vectors. Given two documents 𝑡𝑎→ and 𝑡𝑏→, their cosine similarity can be represented as

𝑆𝐼𝑀𝐶(𝑡𝑎→,𝑡𝑏→)=𝑡𝑎→.𝑡𝑏→∣∣𝑡𝑎→∣∣×∣∣𝑡𝑏→∣∣

  5.4 An efficient movie recommendation algorithm based on improved k-clique:
  
   k-Clique Algorithm: This algorithm used to classify users into several groups.
   
Input: user_training.csv.
Output: group_of_users.
Step 1: initialize mymatrix, sim.
Step 2: for i = 1 to mymatrix do
Step 3: for j = 1 to mymatrix do{
Step 4: initialize a
Step 5: for k = 2 to 4 do
Step 6: if mymatrix[i,k] == mymatrix[j,k]
a[k] = 1
else
a[k] = 0
Step 7: if (a[2]+a[3]+a[4]) == 3
sim[i,j] = 1
else
sim[i,j] = 0 }
Step 8: initialize my_network, k4, b, d
Step 9: for i = 1 to b do
Step 10: for j = 1 to b do d[i,j] = b[[i]][j]



6.Experimental result:

The  results of the experiment depend upon the various values of k After developing the proposed movie recommendation system using improved

k-cliques, the number of movies that were to be rated by the new user among the movies recommended by the system was predicted. Tis paper adopts the most widely used
evaluation metric for performance comparison of the proposed recommendation system. Te mean absolute percentage error (MAPE) is a method of prediction accuracy of
a forecasting method in statistics.
where At
 is the actual value and Ft
 is the forecast value.
 
We compared the MAPE values with the k-cliques method, the maximal clique
method, and the collaborative fltering using k nearest neighbor method to evaluate the
performance.



Conclusions:


In order to achieve more accuracy than collaborative fltering methods; the maximal clique method used in social network analysis introduces in this paper is the first time
that used in a movie recommendation system and the output of this method is veryeffective. To achieve more accurate; the k-clique method, which is very effective in
social networks, is introduced in this experiment and the output showed this methodThe value result of mean absolute percentage error using maximal cliques.

The value result of mean absolute percentage error based on collaborative fltering using a k nearest neighbor was more efective than maximal clique method. Therefore, this report also proposed an
improved k-cliques method to fnd the most efcient method than the k-cliques method.

Finally, after several experiments were performed; in terms of the mean absolute percentage error used to calculate, which is the mean value calculated, the
best method was found when k=11 and rated at least 200 movies with fve movies recommended to the user.For performance evaluation,

we evaluated the collaborative fltering method using a k nearest neighbor, maximal clique method, k-clique method and improved k-clique
methods. The results showed that the improved k-clique method improved the precision of the movie recommendation system more than the other methods used in this.Until now, it takes a long time to calculate the k-clique methods. And data mining method will be used with the improved k-clique method in the future to increase the accuracy and efectiveness of the movie recommendation system.
