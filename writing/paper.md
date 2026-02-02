
## Name

Kushall Saraf

---


### Introduction


In the realm of cutting-edge technology, machine learning (ML) has emerged as a transformative force, revolutionizing various fields with its predictive capabilities and data-driven insights. From healthcare to finance, ML has made significant contributions, enabling more informed decision-making and unlocking new possibilities. One domain where ML's potential has garnered immense interest is sports outcome prediction. By leveraging vast amounts of historical data, sophisticated algorithms, and pattern recognition, ML offers the promise of enhancing our understanding of sports events and ultimately predicting their outcomes with unprecedented accuracy.

Sports, as a multi-billion-dollar industry, has not remained immune to the transformative potential of ML. The vast and ever-growing amount of data generated from sporting events, including player statistics, match results, weather conditions, and more, has become a goldmine for data scientists and sports enthusiasts alike. The application of ML in sports has not only opened new avenues for fan engagement but has also presented opportunities to gain a competitive edge for athletes, coaches, and sports organizations. These teams spend millions of dollars on algorithms used for match outcome prediction, tactical decision-making, player investments, fantasy sports, and injury prediction.[1] The picture below shows the many applications of AI and ML in sports. 

<img width="795" alt="Screenshot 2023-07-30 at 7 03 51 PM" src="https://github.com/LS102-summer2023/project-kushall080206/assets/137182677/28d8a8d0-6ebb-4dcb-9b91-c982de30a476"> [2]

At the forefront of ML applications in sports lies the captivating field of sports outcome prediction. The ability to accurately forecast the results of sporting events has fascinated researchers, data scientists, and sports analysts alike. The implications of successful outcome predictions are multifaceted – from optimizing betting strategies to providing valuable insights for fantasy sports players, and even aiding coaches in devising winning tactics based on an opponent's weaknesses. The below graph shows the trend of ML in sports betting.

![68747470733a2f2f737461746963312e73717561726573706163652e636f6d2f7374617469632f3530366139356262633461613034393161393531633134312f742f3531613535643937653462303066343432383936376536342f313336393739313839363532362f73706f7274732d363230783334392e6a7067](https://github.com/LS102-summer2023/project-kushall080206/assets/137182677/4f869c35-714f-4166-a61d-4c18d392d71c) [8]


In conclusion, the integration of machine learning in sports outcome prediction is a fascinating and dynamic field, holding immense promise for sports enthusiasts, industry stakeholders, and the wider public alike. By harnessing the power of data and advanced algorithms, we endeavour to shed light on the exciting possibilities and potential pitfalls of using ML to predict the unpredictable –outcome of sports events.


#### Research Question

How does the accuracy of Logistic Regression compare to Support Vector Machine (SVM) when used for sports outcome prediction?

#### Motivation

The significance of data-driven decision-making in the field of sports analytics is what inspired this inquiry. Football, being one of the most popular and passionately followed sports worldwide, presents a compelling arena for predictive modelling. The outcomes of football matches are influenced by a myriad of factors, ranging from team composition and player performance to weather conditions and tactical strategies. By comparing the predictive accuracy of Logistic Regression and SVM in this context, valuable insights can be gained to optimize sports outcome prediction models. Understanding which algorithm performs better in forecasting football match results can not only help sports managers and enthusiasts in making informed betting decisions but also provide teams and coaches with valuable pre-match insights to devise winning strategies. 


#### Current State of the Art

The current state of the art in sports outcome prediction using machine learning techniques in football has witnessed significant advancements. Algorithms like ANN, Nearest Neighbors Regression, XGBoost, Random Forest Regression and the ones targeted in this study are majorly used in sports outcome prediction. Algorithms have been widely employed in sports analytics, leveraging historical match data, player statistics, and contextual information to forecast game results. Logistic Regression, a linear classification method, excels in situations where the decision boundary is relatively simple and easy to interpret. On the other hand, SVM, a powerful and versatile algorithm, is adept at handling complex, high-dimensional datasets, enabling it to capture intricate patterns in football data. Many Studies have explored the impact of feature selection techniques and data preprocessing methods on the predictive performance of ML models. However, challenges remain, such as dealing with imbalanced classes and selecting an appropriate kernel for SVM to optimize performance. As the field continues to evolve, researchers aim to fine-tune these algorithms, incorporating advancements in deep learning and ensemble techniques, to achieve more accurate and reliable football outcome predictions. The ultimate goal is to develop models that can enhance decision-making for sports enthusiasts, analysts, and football teams, paving the way for more data-informed strategies and informed sports predictions.


#### Goals of the Project

In this literature review, I delve into the intriguing world of using machine learning for sports outcome prediction. The aim is to explore the various methodologies and algorithms that have been employed to predict the results of sporting events. By analyzing historical data, team compositions, player performance metrics, and various contextual factors, ML models have sought to decode the intricate patterns that influence the outcome of games.

Through this research, I seek to gain a comprehensive understanding of the strengths and limitations of existing ML approaches in sports outcome prediction. Additionally, I aim to identify potential areas of improvement that could further enhance the accuracy of predictions. Furthermore, I will examine how ML-powered predictions are being utilized in real-world scenarios, such as sports betting markets and sports analytics firms, and the impact these predictions have on decision-making processes.



### Related work

[3], developed a logistic regression model to predict match results of Barclay’s premier league. What stands out is that they gathered the significant variables from various research papers rather than just making their own assumptions. They also gathered data from video games like FIFA which they said improved the quality of the data. They used variables like Home Offense,  Home Defence,  Away Offense, and Away Defence. They got a prediction accuracy of 69.5% from their model. They determined that the most significant variables were home Defence and away Defence. 

[4], used the XGBoost algorithm to predict the results using limited data. They proposed a system which uses XGBoost as their primary algorithm for sports outcome prediction. It is compared with other algorithms using a filtered dataset to find the most influential data. Optimization or normalization has been applied, and the predicted outputs will represent win, draw, or loss in human-readable form. They came to the conclusion that XGBoost could outperform many other algorithms.  

[5], set out to predict the results of the Greek league, considered the most predictable league, using 5 machine learning models. These models were as follows: k-Nearest Neighbour (k-NN), LogitBoost (LB), Support Vector Machine (SVM), Random Forest (RF) and CatBoost (CB). They engineered new features from the already existing ones. The following were created: Home Team form (the Home Team’s form according to the last five matches performance of the team), Away Team form, Home Team league points (the points the Home Team has gained in the league for the corresponding season before the match is played), Away Team league points, Home Team previous match goals (the goals scored by the Home Team in the previous match played), Away Team previous match goals, Home Team previous half time match goals (the goals scored by the Home Team in the previous match until half time) and Away Team previous half time match goals. As far as SVM is concerned they concluded they used a few parameters which resulted in an accuracy of 54.07% and the metric results were 0.4258, 0.4414 and 0.3876 for recall, precision and F1-score respectively. According to Table 3 in their paper, SVM had the least accuracy and F1-score. They also used LogitBoost which performs an additive logistic regression. It had an accuracy of 55.65% and an F1-score of 0.4962 ranking 3rd among the five models. The best-performing model was CatBoost with an accuracy of 67.73% which they applied to two more datasets. They concluded that the two most important features were Home Team Form and Away Team Form. Applying the best model to other datasets, they reached the conclusion that each league has its own properties and particularities that need to be considered separately for an accurate prediction. 

[6], modelled an algorithm using Logistic Regression, SVM and XGBoost to compare their accuracy. He used a dataset from the English Premier League. The web scraping was done and datasets from 2000 to 2015 were used. The data was split into training and testing which was then applied to 3 different classifiers and 12 features were considered. After refining the data, the model was run and the F1-score was calculated on the test data. Logistic Regression had a score of 0.6957, SVM had a score of 0.6818 and XGBoost had the highest accuracy with an F1-score of 0.7451. He further ran some tuning parameters which inflated the score to 0.7826. He concluded that adding sentiment from Twitter, and some news articles can improve the accuracy. Also including more features from various data sources could enhance the accuracy of the predictions.

[7], set out to predict the outcome of the NFL (an American football league). He used Logistic Regression and SVM models to execute the project. Scores and statistics from 2003, 2004 and 2005 were used as datasets for the models. For the first algorithm, he used his own implementation of logistic regression in Matlab, which used the Newton-Raphson method. For the second one, he used SVM-light with linear, polynomial and tangent kernels. As for the conclusion the best results were achieved by the Logistic Regression model. The results were as follows – 2005: 65.83% - 2004: 61.37% - 2003: 67.08%. They determined that using the best features with different algorithms can improve the accuracy of the predictions. 

[10], Applying knowledge discovery in databases (KDD) they developed a predictive model for football match results. By analyzing 9 crucial features influencing football outcomes, they constructed a more comprehensive system, resulting in improved prediction accuracy. To achieve this, they employed artificial neural network (ANN) and logistic regression (LR) techniques, utilizing Rapid Miner as our data mining tool. The implemented techniques demonstrated promising results, with the ANN technique achieving 85% prediction accuracy, and the LR technique achieving an even higher accuracy of 93%.

[11], The author developed a system with the aim of surpassing bookmakers' odds in football predictions. The goal was to identify crucial features for match prediction and calculate their probabilities to determine profitable bets. Seven machine learning algorithms, including MultiClassClassifier, RotationForest, LogitbooST, BayesNet, Naive Bayes, and Home Wins, were employed to classify matches into home wins, draws, or away wins. The achieved accuracy of his algorithm was 55%. However, the system fell short of consistently outperforming bookmakers in the long run. A significant limitation of this research was the relatively low prediction accuracy. Subsequently, the author proposed an improved system, which would consider additional features like all bookings during the match, player compositions, team managers, and more.

[12], utilizing player and team data gathered from diverse web sources, the researchers propose an expert system designed to enhance NHL game outcome predictions while also assisting in recruitment and salary decisions. The developed system integrates principal components analysis, nonparametric statistical analysis, a support vector machine (SVM), and an ensemble machine learning algorithm to forecast whether a hockey team will emerge victorious in a game. The ensemble methods exhibit enhancements over the baseline SVM classifier, with predictive accuracy for the testing set surpassing 90%. Through a comparison of various ensemble machine learning approaches, potential avenues for enhancing game outcome prediction accuracy are identified. The system streamlines the application of learning methodologies and inputs data sources for users, facilitates the evaluation of model results, and addresses inherent challenges and concerns in predicting hockey game wins.




#### Threats to Validity

As I have based my conclusion on many research papers, the limitations in those studies will affect my conclusions. Any inaccuracies in the datasets or algorithms used in the various papers may affect the evaluation metrics on which I have drawn conclusions. Factors such as dataset selection bias and sample bias may also act as obstacles in the paper. Data pre-processing choices will also affect the conclusions and in turn affect my conclusions.


### Conclusion

After a lot of literature review, I concluded that Logistic Regression is more accurate than Support Vector Machine (SVM) which can also be seen in the table 1. Though other algorithms perform better than Logistic Regression and SVM, they are out of the scope of this research. I also noticed the importance of feature selection and data processing. I noticed that different algorithms many times reported high accuracies with specific features than with others. Using significant variables can also increase the accuracy to a good extent.

#### Summary of Results

| Ref | Research Title | Dataset | Techniques Applied | Prediction Accuracy |
| --- | -------------- | ------- | ------------------ | ------------------- |
| [3] | Predicting Football Match Results with Logistic Regression | Barclay’s Premier League | Logistic Regression | 69.5% |
| [4] | Football Prediction using XGBoost Algorithm: A Literature Review | NA | XGBoost | NA |
| [5] | Predicting Soccer Outcomes in the Greek League Using Machine Learning | Greek League | k-Nearest Neighbour (k-NN), LogitBoost (LB), Support Vector Machine (SVM), Random Forest (RF) and CatBoost (CB) | SVM – 54.07%, CB – 56.59%, LB – 55.65%, RF – 56.38%, k-NN 50.13% |
| [6] | Predicting Winning Teams | English Premier League | Logistic Regression, SVM, XGBoost | LR – 0.6957, SVM – 0.6818, XG – 0.7451 |
| [7] | Predicting the outcome of NFL games using machine learning | NFL (2003 - 2005) | Logistic Regression and SVM | 2005: 65.83% - 2004: 61.37% - 2003: 67.08% |
| [10] | An Improved Prediction System for Football a Match Result | Match history, Performance index, and match day record | ANN and Logistic Regression | ANN - 85%  LR - 93% |
| [11] | Predicting sports events from past results Towards effective betting on football matches | Home win, draw and away win results | MultiClassClassifier, RotationForest, LogitbooST, BayesNet, Naive Bayes | 55% |
| [12] | A game-predicting expert system using big data and machine learning | NHL.com, ESPN.com, war-on-ice.com, sn.ca, and hockey-reference.com | SVM | 90% |

Table 1




#### Future Work

The field of sports betting is a growing field and there is a myriad of potential work that can be done to get better results in the future. Here is some Future work that can be done in this field:- 

1. Improved Insights Into Player Performance - Gathering more and more data is necessary and with the new technologies it is easier than ever to collect data. Using cameras, microphones, and multiple sensors a lot of different aspects of the game can be recorded. This will increase the number of features available to use for the algorithm's use. [9]

2. Development into other uses - A prediction result can be used to assist the club’s manager to form tactics or strategy for upcoming matches, or it could be developed into a system recommender on what player to buy to strengthen the significant variables in football matches. [3] 




#### Ethical Implications and Recommendations

1. **Transparency and Explainability:** Models developed using machine learning can be very complicated and challenging to understand. Certain models' lack of transparency and may give rise to questions regarding responsibility and the capacity to comprehend the elements influencing forecasts. In order to ensure impartial decision-making, stakeholders, athletes, coaches, and fans, may have a right to know how forecasts are generated.
   
2. **Privacy and Data Protection:** Collecting and analyzing large datasets for sports prediction can involve personal and sensitive information about athletes, team members, or fans. Ensuring proper consent is crucial to protect individuals' privacy and compliance with data protection laws.
   
3. **Fairness and Bias:** Machine learning models trained on historical data can inherit biases present in the data, leading to biased predictions. This may perpetuate existing inequalities in sports, such as favouring well-established teams or players. Ensuring fairness in predictions requires careful consideration of data representation and addressing bias issues.

4. **Integrity of the Sport:** Predicting sports outcomes might lead to potential manipulation attempts by malicious actors seeking to exploit the predictions for personal gain. Maintaining the integrity of the sport is paramount, and measures must be in place to prevent any misuse of models.

5. **Emotional Impact on Fans and Players:** Accurate predictions may heighten the emotional impact on fans and players, potentially leading to increased pressure and stress. Negative effects on mental health and well-being should be taken into account.

6. **Effects on Competitive Balance:** Wide adoption of predictive models in sports decision-making might impact competitive balance. Smaller or less wealthy teams may struggle to compete with larger, more resourceful teams that have better access to sophisticated predictive technologies.

7. **Regulatory Compliance:** Researchers and organizations must adhere to relevant regulations and guidelines regarding the use of ML models in sports prediction, including data protection laws, anti-match-fixing regulations, and responsible gambling practices.

Addressing these ethical implications requires a collaborative effort involving researchers, sports organizations, policymakers, and other stakeholders to develop guidelines, best practices, and policies that ensure the responsible and ethical use of ML in sports outcome prediction.



#### References


[1]  R. Beal, T. J. Norman and S. D. Ramchurn, "Artificial intelligence for team sports: a survey," The Knowledge Engineering Review, vol. 34, 2019. Available: https://www.proquest.com/scholarly-journals/artificial-intelligence-team-sports-survey/docview/2328571462/se-2. DOI: https://doi.org/10.1017/S0269888919000225.

[2]  A. D. Stefano, “Ai in sports: Trends, applications and future challenges,” AI in Sports: Trends, Applications and Future Challenges, https://www.itransition.com/blog/ai-in-sports (accessed Jul. 30, 2023). 

[3]  D. Prasetio and D. Harlili, ‘Predicting football match results with logistic regression’, in 2016 International Conference On Advanced Informatics: Concepts, Theory And Application (ICAICTA), 2016, pp. 1–5.

[4]  W. Gourh, K. N. Poojary, M. Vengarai, and N. Parkar, ‘Football Prediction using XGBoost Algorithm: A Literature Review’, 2020.

[5]  Marios-Christos Malamatinos, E. Vrochidou and G. A. Papakostas, "On Predicting Soccer Outcomes in the Greek League Using Machine Learning," Computers, vol. 11, (9), pp. 133, 2022. Available: https://www.proquest.com/scholarly-journals/on-predicting-soccer-outcomes-greek-league-using/docview/2716507650/se-2. DOI: https://doi.org/10.3390/computers11090133.

[6]  R. Tuwani, “Predicting_Winning_Teams,” GitHub, https://github.com/llSourcell/Predicting_Winning_Teams/blob/master/Prediction.ipynb (accessed Aug. 1, 2023). 

[7]  B. Hamadani , “1. Introduction - Stanford University,” Predicting the outcome of NFL games using machine learning, http://cs229.stanford.edu/proj2006/BabakHamadani-PredictingNFLGames.pdf (accessed Aug. 1, 2023). 

[8]  B. M. LYNCH, Sports Betting to Grow at Double-Digit Rates over the next Five Years. AUSTRALIAN RACING FACTBOOK. 

[9]  “The future of AI in Sports Betting,” BettingGods.com, https://bettinggods.com/sports-betting/the-future-of-ai-in-sports-betting/ (accessed Aug. 1, 2023). 

[10]  C. P. Igiri, ‘An Improved Prediction System for Football a Match Result’, IOSR Journal of Engineering, vol. 04, pp. 12–020, 2014.

[11]  D. Buursma, ‘Predicting sports events from past results Towards effective betting on football matches’, 2011.

[12]  W. Gu, K. Foster, J. Shang, and L. Wei, ‘A game-predicting expert system using big data and machine learning’, Expert Systems with Applications, vol. 130, pp. 293–305, 2019.

