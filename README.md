# Student_scores_EDA_ML
On this project the data from the Kaggle's Database kaggle datasets students-performance-in-exams. It is a sintetic generated dataset of students scores in 3 subjects(Maths, Writing and Reading). 

The target of this analysis was: "Identify the features that affect the students scores each exam and make recommendations to decrease the number of fail students". 
The pass or fail treshold was set at 50. To identify the the features that affect the scores, there were used an EDA analysis and 2 machine learning models (Logistic Regression and Random forest). The logic of the analysis with this machine learning models was: 
- Train the model on the features to classify the students that pass and do not pass the exam.
- Evaluate the importance of each feature in the model. So the features with higher importance(weights) in the model, are the features that most affect the students in order to pass or fail the exam

By this logic, the target of the analysis is not get the model with the higher accuracy, but evaluate the feature importances(weights) in different models to make a conclusion and recommendations for the decrease of students that fail the exam. Because of this there were only applied Logistic regression and Random Forest, as they let us to see the feature importance(weights) of the model.

In the case of the Random Forest, defferent seeds of ramdoness were used, as on each seed, the model uses diferent features to make the prediction. This allow us to make a deeper analysis on the features correlation with the exam score. For example was found that the model can use either the parents level of education, either the type of lunch of the students and get similar accuracies. This let us the hipothesys that there is a correlation between the both features, and its not the parent level of education the reason of fail an exam, but the fact that parents with higher level of education give their childrens better lunch,  and lunch is the reason of decrease or increase in the exam scores 

The work was divided in 2 :
1. The EDA analysis maked for each exam score, all in one notebook. It can be seen in the Students_EDA_Analysis notebook in EDA_analysis folder
2. The Machine learning models to evaluate feature correlation with each exam score separately. For each exam score there is a notebook in the ML_models_feature_analysis folder
