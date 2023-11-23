# Insurance_premium_prediction

The goal of this project is to give people an estimate of how much they need based on
their individual health situation. After that, customers can work with any health 
insurance carrier and its plans and perks while keeping the projected cost from our 
study in mind. This can assist a person in concentrating on the health side of an 
insurance policy rather han the ineffective part.


**Conclusion:** 

* When we tried multiple regression algorithms , we got "GradientBoostingRegressor" gives the best result among all the models & Model Score is 0.866
* By performed hyperparameter tuning using GridSearchCV to get best parameters
* Best parameters for this model is :
    * learning_rate: 0.1
    * loss : squared_error
    * max_depth: 2
    * min_samples_leaf: 1
    * min_samples_split: 6
    * n_estimators: 100
* Our Best Model Score is:
    * Train: 0.878 - Model is able to explain approximately 87.8% of the variance in the training data.
    * Test:0.871 - Model is able to generalize and make accurate predictions on new, unseen data is 87.1%.
    * As train & test scores are very near , we can conclude our model is not overfit & also has the potential to genaralize well.
* Importence of features:
    * Age" feature doesn't contribute significantly to the predictions.
    * The "BMI" feature has a small positive importance, indicating a minor contribution to the model's predictions.
    * "Children" has the highest importance, suggesting it plays a significant role in the model's predictions.
    * The "Sex_female" feature has a higher importance compared to "Sex_male," indicating that gender, especially female, is considered important in the model.
    * Among the regions, "Region_southeast" has the highest importance, indicating it has a stronger influence on predictions compared to the other regions.
