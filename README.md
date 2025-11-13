# Bayern Munich Match Outcome Prediction



###### This project uses historical football match data from the European Soccer Database to predict whether FC Bayern Munich will win the league in a given season using machine learning.



## Dataset:



###### The project is based on the European Soccer Database (SQLite), which includes:



* Match.csv — match details (scores, teams, dates)
* Team.csv — team information
* Team\_Attributes.csv — team stats and attributes across seasons



## Project Workflow:



#### 1\. Data Preparation



* Loaded match and team data from CSV files.
* Filtered only matches involving FC Bayern Munich.
* Merged Bayern’s match data with corresponding team attributes.
* Created numeric features such as:

buildUpPlaySpeed, chanceCreationPassing, defencePressure, etc.



#### 2\. Feature Engineering



* Encoded match results as binary outcomes:

&nbsp;	1 → Bayern won the match

&nbsp;	0 → Bayern did not win

* Dropped irrelevant or non-numeric columns (like season strings).



#### 3\. Model Training



* Split the data into training and test sets.
* Trained a Random Forest Classifier to predict match outcomes.
* Evaluated performance using:

&nbsp;	Accuracy

&nbsp;	Confusion Matrix



#### 4\. Results



* Accuracy: 1.0
* Confusion Matrix:



\[\[1 0]

&nbsp;\[0 1]]





* Confidence (Win League): 0.58



#### Visualizations



* Correlation Heatmap to understand feature relationships
* Feature Importance Plot to show which team attributes influence Bayern’s performance the most





#### Model Used



* Random Forest Classifier

&nbsp;	Chosen for:



* &nbsp;		Handling both numerical and categorical data



* &nbsp;		Low risk of overfitting



* &nbsp;		High interpretability with feature importances

#### 

#### Future Improvements



* Add more advanced models (e.g., XGBoost, LightGBM).
* Use match-level attributes for both home and away teams.
* Incorporate player stats for deeper analysis.
* Predict match scores instead of binary outcomes.



#### Requirements



pip install pandas numpy matplotlib seaborn scikit-learn



##### Author



Habiba Zaki

Machine Learning Student | Data Science Enthusiast

