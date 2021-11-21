# Josh Galloway Portfolio
I have produced multiple accomplishments by designing, implementing and testing a wide range of control functions, providing process modeling solutions, and leveraging the power of technology to solve challenging problems. Success includes managing priority projects by applying strong communication, leadership and influencing skills. I received my M.S. in Applied Mathematics focusing on Data Science in May of 2021, adding to a B.S. in Electrical Engineering (2008). I'm currently working as Data Scientist after a lengthy career as an Advanced Process Control Engineer. 

#### [LinkedIn](https://www.linkedin.com/in/josh-galloway/)
#### [Resume](https://github.com/jgalloway42/JoshG_Portfolio/blob/main/Josh_Galloway_Resume.pdf)

## [RNN/NLP Application: Predicting VIX Ticker Volatility from Headlines](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/Math_7243_Machine_Learning_Final_Project_r3.pdf)

Working from publicly available data sources, the student trained a recursive neural network (RNN) implemented in Python (pandas, sklearn, keras) to predict the Chicago Board Options Exchange (CBOE) Volatility Index (VIX). An ad hoc method of sentiment quantification was applied to datasets containing Reddit and ABC headlines spanning several years. The result was a trained RNN that was able to predict the Delta VIX closing day over day based on the headlines from the previous 20 trading days.
<br>
Once  trained,  the  network  was  scored  against  a  test  set  to  root-mean-squared  error (RSME),  and  evaluated  again  by  graphing  the  results  of  the  prediction  against  the recorded  data  set.   The  RMSE  was  1.87  for  the  ABC  dataset  against  the  segregated test set, and 2.07 for the Reddit.  The predictions graphed against the ABC datase is shown below.

![](/images/VIX_Prediction_ABC_Headlines_Results.png)

## [Unsupervised Learning, NLP, Clustering: Clustering of News Headlines for Sentiment Analysis](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/DS%205230%20Unsupervised%20ML/Galloway-DS5230-Final%20Project%20Report.pdf)
The goal of the project was to analyze a collection of news headlines to identify reoccurring sentiment themes. The dataset was comprised of roughly 1.25 million headlines and is the synthesis of two datasets publicly available on Kaggle. The news sources from which the headlines were pulled were Reddit’s WorldNews channel and ABC which is an Australian news organization. The time span for the collective dataset was roughly from 2003 to 2019. This project utilized skills in natural language processing (NLP) and unsupervised machine learning techniques in clustering analysis.  Several clustering and preprocessing techniques were evaluated to find the best method and number of sentiment clusters.
![](/images/UML_TF_TFIDF_Wordcloud.png)

The K-means LDA-based model performed best based on Silhouette coefficient and CH score metrics.  In fact, the LDA-based models performed better in all cases with the exception of DBSCAN.  This is likely due to the additional sophistication in the LDA algorithm from the inclusion of extra latent variables versus the non-negative matrix factorization.

![](/images/UML_KMeans_LDA_3d_views.png)

Comparing the models in a confusion matrix shows only a few labels were in disagreement. Inspecting these disagreements on a PCA-reduced two dimensional graphing of the LDA dataset clarifies the region of disagreement for all the algorithms is generally between the boundary of cluster 0 and 3.  Inspecting the topics closest to the Cluster 0 and 3 centroids shows that the two topics are slightly similar with the words ‘fear’ and ‘warns’ and other vaguely worrisome words associated with each topic.

![](/images/UML_confusion_matrtix.png)

The reserved test set was utilized to measure the performance of the model. Using only words from the model’s 2000 term vocabulary, the headlines in the test set were scored for sentiment; following which, the K-Means model was used to predict a label for each headline. Each randomly selected 50-point testing fold was scored on Silhouette coefficient and CH score.  The CH score distribution was very tail heavy showing high levels of clustering performance for a significant portion of the folds.  The box plot for the CH score distribution shows many outliers to the higher performing side of the interquartile range.  The Silhouette coefficient distribution was shown to be roughly normal with a mean score of 0.66 and 95% confidence interval from 0.55 to 0.76.

![](/images/UML_CI_Bootstrapping_Results.png)

In both cases, the scoring was improved on the test set over the training score. This is likely due to duplication of topics between headlines creating tighter clusters with more distance between them, as this would improve either metric.

## [Anomaly Detection with Local Outlier Factor Study](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/DS%205230%20Unsupervised%20ML/14_Module%20Final%20Exam/presentation/Galloway-DS5230-Final%20Exam-Local%20Outlier%20Factor.pdf)

A study of varying methods for anomaly detection with focus on implementation and detailed examination of the Local Outlier Factor method as compared to other major clustering methods.

![](/images/LOF_vs_Others.png)

## [Classification of Obesity Levels](https://github.com/jgalloway42/classification_of_obesity_levels)

Utilizing a publically available data set, this project builds a classifier of obesity level between levels (Insufficient Weight, Normal Weight, Overweight Level I, Overweight Level II, Obesity Type I, Obesity Type II and Obesity Type III) based on eating habits and physical conditions of the individuals. Four models were optimized via grid search and 5-fold cross-validation: One vs Rest Logistic Regession, One vs Rest Support Vector Classifier, Random Forest, and XGBoost and scored on macro averaged F1 score. Overall, both the random forest and XGBoost model performed very well with f1-scores over 95% in both cases. The resultant confusion matricies follow:

![](/images/obesity_combined_cf.png)

## [XGBoost Sales Forecasting](https://github.com/jgalloway42/xgboost_sales_forecast/tree/main)

The project comprises data formating, feature engineering, EDA and optimization of an XGBoost regressor via gridsearch.  Overall the forecasting produced very good results with an R<sup>2</sup> of 0.87.

![](/images/Prediction_Results_Close_Up.png)

## [Markov Chain Modeling: Wind Speed Data from Boston Logan Airport](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/MATH%207241%20Probability%20Models/Math_7241_Markov_Chain_Project.pdf)
Wind speed data from Boston Logan Airport was analyzed and modeled utilizing python/matlab and the model was evaluated via Chi-squared test for the two-step expected values. The choice of model was required as part of the graduate level course, and is a poor fit as applied due to the seasonality inherent in the data. However, the results were reasonable.
<br>
![](/images/BWSnetworkGraph.png)
<br>
![](/images/BWStwo_step_frequencies.png)

## [Computer Vision: Real Time Liquid Level Detection](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/GallowayMath7203MiniProject01_Notebook.pdf)

A from scratch implementation of the Canny Edge Detection Algorithm in Python utilizing numpy was modified to track liquid level in a vessel as it was drained from a vessel.  The resulting system worked very well. The gif below runs very slow compared to the real implementation, but is shown to elucidate the concept.

![](/images/liquid_level_tracker.gif)

## [Cart-Pendulum System Dynamic Simulation and Control](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/Math_7203_Mini_Project_II_Cart_Pole_ODE_Simulation.pdf)

Project descriptionThe dynamics of the classic cart-pole system were simulated using the Python language's available initial value problem (IVP) ordinary differential equation (ODE) solver. The system was animated to allow for visualization and verification. Following this, the system was linearized around an equilibrium point to allow application of linear control theory; then, a Linear Quadratic Regulator (LQR) was constructed to control the system. The controlled system was simulated and animations produced once again to verify accuracy of the results.

*Uncontrolled simulation*
<br>
![](/images/CartpoleSimNoForcePendOffCenter.gif)
<br>
*Controlled simulation with objective to center cart and balance the pole*
<br>
![](/images/CartpoleSimOptimalControl_objective_cart_x_to_0.gif)

## [Nonlinear Ordinary Differential Equation Simulation: Hodgkin-Huxley Neuron Action Potential Model](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/MATH%207205%20Numerical%20Analysis%202/Project%2001/Galloway-Math%207205%20Mini-Project%2001%20Presentation.pdf)
The Hodgkin-Huxley Model was implemented/simulated in python/numpy utilizing Forward Euler, Huen's Method and 4th order Runga-Kutta all of which were coded from scratch.
![](/images/HHM_rk4_simulation.png)

## [Linear Programming Optimization of Industrial Cogeneration Facility Operation](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/MATH%207205%20Numerical%20Analysis%202/Project%2002/Galloway-MATH7205-MiniProject-02-Presentation.pdf)

The steady state operation of a cogeneration facility was simulated in python and then, utilizing scipy and cvxopt's linear programming functionality, optimized under varying operational conditions.
![](/images/OptimizationResultMaxSteamOffset.png)

## [Industrial Boiler Drum Dynamic Modeling and Simulation](https://github.com/jgalloway42/MS-Applied-Mathematics-Projects/blob/master/Galloway-Final%20Project%205131-Paper.pdf)
A first principles model of an industrial boiler drum was created and simulated numerically in Python to examine the shrink-swell phenomenon.

![](/images/boiler_drum_shrink_swell.png)

## [HONORS UNDERGRADUATE RESEARCH: AUTONOMOUS ROBOT FOR REMOTE DETECTION OF UXO](https://github.com/jgalloway42/BSEE_papers_and_projects/blob/master/Galloway_thesis.pdf)

The Electrical and Computer Engineering Technology (ECET) Honors student developed a prototype for an autonomous landmine and unexploded ordinance (UXO) seeking robot. The system provided functionality including locating metallic landmines and UXO within a defined area/environment, recording the location of said landmines and UXO’s, and storing the data off unit via an IEEE 802.11b/g connection to a Windows or Linux-based personal computer. The project afforded the student the opportunity to explore the field of robotics with the added benefit of providing experience with mechanical systems,printed circuit board (PCB) layout/production, and network programming in Java. Application of the prototype and corresponding research may lend themselves to demining the more than 100 landmine/unexploded ordinance affected countries in the world particularly in desert terrain (US Department of State Fact Sheet, 2 July 2003).
![](/images/undergrad_robot.png)
