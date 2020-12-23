# Fifa_Player_Position
Visualization and Classification of Soccer Players

In soccer or football as it is more commonly known, the objective of every team is simple. That is to win by scoring more goals against the opposition while conceding less within a 90 minute game. Although the objective may seem straightforward from the outside, there are a lot of details that needs to be worked on behind the scenes to win games.
One of the main factors that increases a team’s chance at winning games is player selection, more specifically, having the players with the right physical and technical attributes in the right places. In a team, there are eleven players that have their own unique positions on the field. Excluding the goal keeping position, there are ten outfield players that can be grouped by their commonalities. In this paper we take a look into the four most important positions in soccer. These positions include Center Backs (CB), Full Backs (FB), Center Midfielders (CM) and Strikers (ST). First we will explore Principal Component Analysis (PCA) and K-means clustering to visualize our data in detail. Then, a classification approach is introduced to classify a player’s position based on their given features using a trained Random Forest (RF) and a Support Vector Machine (SVM). This model has could potentially be very useful in helping a coach scout and pick the best players for his team to ultimately increase their chance of winning.

The data used in the visualization, training and testing of the aforementioned models was obtained from kaggle.com (a crowd- sourced, data-sharing platform), is owned by Karan Gadiya, and was scraped from the videogame, FIFA 19. The data reflecting the attributes of thousands of players is legitimate and influenced by their actual performances in matches. The original dataset contained data for players in every position but for this project, a subset of the original dataset was taken by only selecting the outfield players. The outfield players were then grouped into four main positions.
This dataset contains 21 features and 11,829 cases, where each case is a player. Out of the 21 features, only one is a categorical feature.

In terms of the number of classes, the dataset contain four classes and they span across all the outfield positions. The trained machine learning algorithms will use the features listed above to classify each case to a position. The classes “CB”, “FB”, “CM” and “ST” populate about 26.1%, 23.5%, 22.5% and 27.9% of the dataset respectively. Since the classes are not extremely imbalanced, implementing more balancing techniques was not required.
