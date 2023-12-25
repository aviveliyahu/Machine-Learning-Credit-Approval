# Machine Learning - Credit Approval using big data environment
## IMPORTANT NOTE: Github has an issue supporting visualization so we added them as a jpeg file to the repo, you can use the file in your spark / databricks environment in order to view it right. in the right environment the visualization is dynamic and responding to mouse hover / click.


## Description
This is a final project using big data tool such as spark and databricks and make use of our knowledge in Python, Machine learning algorithms and workflow (using Pipeline, OneHotEncoder etc..) , Databricks environment and data analysis tools.
We were asked to check a known machine learning algorithms in order to predict wether to approve or not the user's credit card.
We were given a dataset that we had to import as a Pandas dataframe, explore the types of columns it has and check if there are missing values or other parameters that need to be fixed.
Later, we had to create our machine learning models, in our project we checked the following- 
* Logistic Regression
* Random Gorest
* Decision Tree
* Gradient Boosting
* Support Vector Machine
* Logistic Regression
* Factorization Machine

In order to make sure that the results are correct and we didnt have just proper luck for splitting test and train data, we tested each model 10 times (each iteration we randomly split the train and test data) and re-fit the models again to provide more accurate and real results for each model.
Some columns were strings so we had to transform them into a vector so we would be able to fit the models the data without losing important information. we used OneHotEncoder and StringIndexer in order to do so. After that we combined it all into one long vector.
Since we have many models, and each time we had to use OneHotEncoder to solve the tring columns, we used Pipeline technique to do it automatically each iteration.
After doing so, we saved each model's data in order to create a confusion matrix - later on we transformed it into a dataframe and combined them into one big dataframe.

The dataframe we created helped us to give insights about the models, and choose the most effective model in our case of credit approval (considering that we need to make sure the accuracy is one of the most important parameters).
After choosing the model (Random Forest) we started to dive in and see which parameter has the most impact on wether to approve or not the credit for the costumer.
We had a conclusion that the most important feature that affect it was wether the costumer had any previous default to his credit card, secondly was his working status and time he work in the same place and lastly the current credit score he has.
We also gave a small advice to the 'imaginary' credit approval company on how to approve or not a new costumer and what to look for the most.


### Notes
Github has an issue supporting visualization so we added them as a jpeg file to the repo, you can use the file in your spark / databricks environment in order to view it right. in the right environment the visualization is dynamic and responding to mouse hover / click.


## Authors

Contributors:

[@Aviv Eliyahu](https://github.com/aviveliyahu)
[@Ariel Goldwaser](https://github.com/ArielGold1)
[@Matan Asraf](https://github.com/matanasaraf)
