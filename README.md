Introduction
------------

This is my 3rd machine learning project. The project is Language Dtetection. Language plays an important role in our daily lives, without it we won't be able to coordinate with other or express our feelings, but we cannot learn every lamguage present out there as it's too tidious. So, our aim is to build a language detecxtion model that can detect the langauge in which any textual data is written. Earluer, it wasn't possible for machines to process such vast data due to limited machinery and space but as the machine advanced we can see this model being implemented all around the world, the best example of such model is Google's Language Detection which we all might have used once. So, our aim is to build the same model and predict the language in which the textual data is present.

Dataset
-------------
The dataset I've taken is from Kaggle and can be accessed with the given link: https://www.kaggle.com/datasets/basilb2s/language-detection
The dataset contains 10337 rows/instances and 2 columns, the dataset is quite simple, the columns or features present in the dataset are: 
1. Text: This column represents the textual data in which the data is written. The textual data in many languages.
2. Language: This column represents the laguage in which the textual data is written.

This dataset will work as a training set for the model we're building. So, this was all about the dataset. 

Data processing
---------------
Now we'll see if there are any null/missing values in our dataset. If there appears ot be any null values then we will have to drop or add them via data pre-processing. But there are no null/missing values in the dataset. Hence, we can move ahead with the building of our model. 

Now I notice all the languages present in the dataset, there are 17 languages present in the dataset with different distribution of their textual data. 'English' language has the higheest number of examples (1385) and language 'Hindi' has the lowest number of examples (63). 

Model Building
---------------
Now that we have processed the data, it's time to move ahead with the building of our language detection model. The problem is related to Multiclass Classification hence I've used Multinomial Naive Bayes algorithm to train the model using our datase with multiple languages present in the dataset. 

Now I've split the data into training and testing sets. 

So, we've successfully trained our model and the accuracy of our model appears to be 0.977 which is quite good. 

Testing of the model
--------------
Now it's time to test our model, and we cann do so by taking the input from the user and then run that inout in our model, the model should be easily able to detect the language in which the user has presented the input. 

Conclusion
------------
Here we can see that the model is able to detect the language in which the user is typing the inout but there are certain limitations, the model is able to detect only 17 languages that were present in our dataset and the model is presenting random results for the languages where less examples were present such as 'Hindi' language. 
So, this was our model and some limitations with it. Such limitations can be resolved by taking a dataset with a vast number of instances. So, that was all about this project. 
If you wish to connect on Linkedin, here's the link: https://www.linkedin.com/in/piyush-goel-6974b4203/
