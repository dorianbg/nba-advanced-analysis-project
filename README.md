# Submission for Data Madness (Data Analysis course)    

Authors: Dorian Beganovic, Presian Abarov     

Video: https://youtu.be/XHsbQNyn44c   

The source code can be found in: DataMadness.ipynb    

# Abstract

NBA (National Basketball Association) is the most popular basketball league in the world. We analyzed shot logs from 2016-17 regular season containing every shot each player took during that season along with some descriptive features. We aimed to analyze how the best and worst teams at scoring differ. Namely we compared the Golden State Warriors with Philadelphia 76ers. We visualized the shot distribution on the court of each team. Shots were clustered to 12 different centroids. Centroids were generated using probabilistic clustering models - Gaussian Mixture Model. Each centroid has a mean and corresponding variance. The variance is represented as ellipses on our charts. We also plot the accuracy of shots from each cluster. The representation allows a skilled analyst to quickly spot the differences between teams. We noticed that main difference was that Golden State Warriors shot at a higher percentage mid-range and three-point shots as well as take more three-point shots.    

Secondly, we analyzed whether the hot hand fallacy is valid. The hot hand fallacy is a belief that a person who experiences success with a random event has a greater probability of further success in additional attempts. We introduced a streakiness metric that extracted the current streak of successfully made shots from the last 15 shots of a player. Through a barplot we saw that the probability of making a shot indeed continuously rose after a streak of length 5. To further investigate this we plotted a histogram of distribution of streak lengths and found that streaks longer than 5 were very rare. Then we plotted the relative distance of a shot along with the length of a streak and found that shots longer streaks were always made closer to the basket and those are usually very high probability shots. We concluded that longer streaks only happen with players shoot often near the basket and that the hot hand fallacy is not valid when players keep shooting at normal distances.    

Lastly, we aimed to create guidelines for predicting whether a shot of a player would go in based on the shots features such as location. We build a specific model for player Kevin Durant who is often regarded as the best scorer. Decision trees offered a natural solution to this problem and we trained a decision tree and visualized the resulting decision true that could guide a decision making process. The model had solid accuracy of 68% which is improvement compared to random guessing. The most important features of the model were also important for analysis and we found some interesting findings such as whether the last opponent shot was blocked was very indicative if Kevin Durant will score on his shot. We assume this is because after a blocked shot the team can score the basket in transition where Kevin Durant is one of the best finishers. We also found that features like where the game is played (at home or on the road) were very important.

