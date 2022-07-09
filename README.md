# Domestic Violence Prediction Project

![](Domestic-Violence-and-Children.jpeg)

The rise of social media has contributed to an emergence of a virtual agora, where mass collection of textual data representing social and political attitudes is now possible through APIs. With the popular usage of social media as sources of mental health support, this is also applicable to the topic of domestic violence. 

In this project, we analyze text data from Reddit and Twitter APIs to predict two cases respectively: (A) whether or not a conversation pertains to the topic of domestic violence; and (B) whether or not a person is likely to stay or leave an abusive situation based on the language they use. 

The NLP models used in these predictions can be applied to an alert system in online therapy algorithms such as 7 Cups, where volunteers may not be fully trained to recognize when to refer the patient to a registered therapist. The feature importances can further contribute to a broader understanding of the narratives of people who are likely to stay in abusive relationships. 


In this folder:

1. Reddit Shelved Data
	This pulls data from precompiled python shelves from [Nicholas Schrading's website](http://www.nicschrading.com/data/). We specifically used the even small set of submissions and comments datasets but there are others available. 

2. Reddit EDA 
	Exploratory data analysis done with the exported data from (1), which involves cleaning, visualization, preprocessing, and tokenization for future modeling. Also uses the [Emotions Sensor Data](https://www.kaggle.com/datasets/iwilldoit/emotions-sensor-data-set) for preliminary emotion analysis. 

3. Reddit Modeling
	This tests three popular models used for NLP: Naive Bayes Classifier, Random Forest Classifier, and Logistic Regression. Best parameters are tested with `GridSearchCV` and feature importances and thresholding for the best model are shown. 
	
4. Twitter API 
	This pulls data from the Twitter API using the code from [Schrading's website](http://www.nicschrading.com/data/).  *must use own personal access token*

5. Twitter EDA
	Exploratory data analysis done with the exported data from (4), as in the Reddit EDA notebook.

6. Twitter Modeling
	This also tests the same three models with `GridSearchCV` and shows the feature importances and thresholding process as in the Reddit modeling notebook. 

7. Report
	A 21-page report summarizing (1) to (6).

8. Slides
	A 24-slide presentation for the findings above.


Reference papers: [Reddit paper](https://aclanthology.org/D15-1309.pdf), [Twitter paper](https://aclanthology.org/N15-1139.pdf)

Data: [Reddit & Twitter Data](http://www.nicschrading.com/data/) [Emotions Sensor Data](https://www.kaggle.com/datasets/iwilldoit/emotions-sensor-data-set)