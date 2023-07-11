# Sports Analytics (Research Project : 753A01)

## Replacement for Chris Gayle in IPL based on Machine Learning algorithms 

Cricket is a game of uncertainty, and it has the second-highest fan base in the world after Soccer. Many models have been constructed to predict the performance of players and a few about classification techniques as well. This project deals with a specific problem of exploring options for replacing CH Gayle, an explosive batsman cum all-rounder, at the Indian Premier League(IPL). A combination of unsupervised and supervised machine learning algorithms have
been implemented to find relevant players who can replace Gayle in the tournament. Moreover, it has been attempted to rank the choice of players in the selection list based on performance and given conditions. Overall, this study tries to build, compare and shortlist a model with higher accuracy, which can group similar players based on past performance and predict their contribution to reason about order of selection.

## Data and Tools
The study utilized Kaggle's ball-by-ball and match datasets of IPL, containing 193,468 balls and 816 matches respectively. The data was cleaned, categorized into Batsman, Bowler, and Fielder groups, and merged for analysis. R-studio, Weka, Google Colab, and Python were employed for data pre-processing, clustering techniques, feature analysis, supervised machine learning, and prediction.

## Batsmen, Bowler, and Players attributes 
Batsman attributes were analyzed using Weka's Filter method and Ranker algorithm, resulting in a ranked list of attributes including Date, Bowling team, No 4s, Batting team, No 100, Runs scored, No 6s, and more. The least important attribute, ID, was discarded due to minimal impact and computational requirements.

In T-20 cricket, bowlers face challenges due to limited overs and aggressive batting. The study divided wickets taken into smaller categories to enhance prediction accuracy.

Player attributes combined batting, bowling, and fielding attributes, and Weka analysis provided a ranked list of attributes such as No matches, Batting avg, No 4s, Runs scored, Innings played, and more. The dataset was scaled and a distance matrix visualization was used for unsupervised clustering.

## Algorithms and its Implementation
### Classification (Unsupervised machine learning)
Cluster analysis is an unsupervised machine learning technique that groups data objects based on their similarity. This study utilized popular clustering algorithms such as K-means and Hierarchical clustering to determine the ideal clusters for players in the IPL dataset. The Gap statistic method suggested dividing the dataset of 170 players into 9 clusters as an optimal choice to avoid generalization. Moreover, These two clusters (Kmeans and Hierarchical) looked identical and listed the same players. It was concluded that the clustering techniques performed really well and did not provide any conflicting results.

### Learning Algorithms (Supervised Machine Learning)
The supervised machine learning models were used for generating the prediction models. The labeled dataset is used to train the model, and then it predicted results for the input features. In this study, the target datasets were the Runs_category and Wickets_category used to find two different models for batting and bowling, respectively. The study used popular algorithms such as Naïve Bayes, decision trees, and random forest to find the best-suited model for the purpose.

## Model Performance 
The SVM and Random forest (98.21%) performed the best as the Batsman model predicting Runs, while SVM (72.41%) predicted best in the wickets category. These two models were used on the players clustered along with Chris Gayle, to predict their runs and wickets points. The aggregations were made to list the overall top 3 players that can replace Chris Gayle in case of his retirement. 

## Conclusions
In order to respond to the research question, the top three players that can replace Chris Gayle in IPL were Shane Watson, Kieron Pollard, and Yuvraj Singh in the respective rank of choice based on clustering and performance of the predictive model.

## Limitations
The study had a few limitations as many factors were not accounted such as current form, weather factor, compatibility with team members, and age-based performance.   

## Future Work
The study could be applied to other players in cricket for whom a franchisee may look out for replacement with inclusion of other important factors as highlighted in limitations. This study could also extend to other sports as well, such as kabaddi, football, etc.

