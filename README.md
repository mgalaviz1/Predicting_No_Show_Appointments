![Picture1](https://user-images.githubusercontent.com/35669027/106232266-92898300-61c1-11eb-8596-ad4b5b00da09.png?raw=true "Optional Title")

# Predicting No-Show Appointments

This project compares 5 different supervised models to determine which best predicts patient no-shows. Accurately predicting when a patient will fail to show up for an appointment allows more efficient overbooking of appointments, better staff utilization and increased ROI for the clinic or hospital. The best model is chosen according to the best F1 score, recall and accuracy scores.

The data can be found at Kaggle https://www.kaggle.com/joniarroba/noshowappointments

The data contains 14 features about 110,000 observations (appointments) in Vitoria Brazil between 29 April and 7 June 2016. 

Weather data was added and analyzed to determine any possible effect weather may have on whether patients will miss there appointments. No significant difference was detected probably due to the brief period being analyzed and, additionally, because it rained only 1 day during business hours contained in this dataset. 

After balancing the target variable and modeling classifiers XGBoost, Support Vector Classifier, Random Forest, kNN and logistic regression for highest recall score, all the models performed about the same. However, all performed better than a dummy model or random guessing. Results indicate that the clinics in the dataset could save about $400 per day assuming $200 cost for each appointment. 

The results are biased because of the very short timeframe which is about 6 weeks. Preferrably, data would be long enough to reflect how weather impacts people showing up for their appointment especially in dense urban environments such as Vitoria Brazil where people are likely to take public transportation to their appointment versus more suburban locations where weather may have less impact. Clinic specialty and subspecialty may have in important role as well since pediatrics may tend to have lower missed appointments since parents tend to be good at getting their kids to a doctor. Age may play a role to if seniors have more time and incentive to leave the house to get to their appointment. Generally, we need to collect more data and for a longer period of time. 
