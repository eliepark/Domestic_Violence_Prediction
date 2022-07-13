# Domestic Violence Prediction Project

![](https://dedwardslaw.com/wp-content/uploads/Domestic-Violence-and-Children.jpg)

The rise of social media has contributed to an emergence of a virtual agora, where mass collection of textual data representing social and political attitudes is now possible through APIs. With the popular usage of social media as sources of mental health support, this is also applicable to the topic of domestic violence. 

In this project, we analyze text data from Reddit and Twitter APIs to predict two cases respectively: (A) whether or not a conversation pertains to the topic of domestic violence; and (B) whether or not a person is likely to stay or leave an abusive situation based on the language they use. 

The NLP models used in these predictions can be applied to an alert system in online therapy algorithms such as 7 Cups, where volunteers may not be fully trained to recognize when to refer the patient to a registered therapist. The feature importances can further contribute to a broader understanding of the narratives of people who are likely to stay in abusive relationships. 

In the near future, chatbots may be used to train people to outgrow their patterns of abusive history, whether they are a victim or the abuser. AI can be trained to pick up language used by people who are likely to stay in an abusive situation, and in turn, promote the narrative of people who are likely to leave.


In this folder:

1. [Report](https://github.com/eliepark/Domestic_Violence_Prediction/blob/main/Report.pdf)
	
	- A 21-page report summarizing (3) to (8).

2. [Slides](https://github.com/eliepark/Domestic_Violence_Prediction/blob/main/Slides.key)
	
	- A 24-slide presentation for the findings below.

3. [Reddit Shelved Data](https://github.com/eliepark/Domestic_Violence_Prediction/blob/main/Reddit_Shelved_Data.ipynb)

	- This pulls data from precompiled python shelves from [Nicholas Schrading's website](http://www.nicschrading.com/data/). We specifically used the even small set of submissions and comments datasets but there are others available. 

4. [Reddit EDA](https://github.com/eliepark/Domestic_Violence_Prediction/blob/main/Reddit_EDA.ipynb)

	- Exploratory data analysis done with the exported data from (3), which involves cleaning, visualization, preprocessing, and tokenization for future modeling. Also uses the [Emotions Sensor Data](https://www.kaggle.com/datasets/iwilldoit/emotions-sensor-data-set) for preliminary emotion analysis. 

5. [Reddit Modeling](https://github.com/eliepark/Domestic_Violence_Prediction/blob/main/Reddit_Modeling.ipynb)
	
	- This tests three popular models used for NLP: Naive Bayes Classifier, Random Forest Classifier, and Logistic Regression, on the processed dataset from (4). Best parameters are tested with `GridSearchCV` and feature importances and thresholding for the best model are shown. 
	
6. [Twitter API](https://github.com/eliepark/Domestic_Violence_Prediction/blob/main/Twitter_API.ipynb)
	
	- This pulls data from the Twitter API using the code from [Schrading's website](http://www.nicschrading.com/data/).  *must use own personal access token*

7. [Twitter EDA](https://github.com/eliepark/Domestic_Violence_Prediction/blob/main/Twitter_EDA.ipynb)
	
	- Exploratory data analysis done with the exported data from (6), as in the Reddit EDA notebook.

8. [Twitter Modeling](https://github.com/eliepark/Domestic_Violence_Prediction/blob/main/Twitter_Modeling.ipynb)
	
	- This also tests the same three models on the data from (7) with `GridSearchCV` and shows the feature importances and thresholding process as in the Reddit modeling notebook. 




Reference papers: [Reddit paper](https://aclanthology.org/D15-1309.pdf), [Twitter paper](https://aclanthology.org/N15-1139.pdf)

Data: [Reddit & Twitter Data](http://www.nicschrading.com/data/), [Emotions Sensor Data](https://www.kaggle.com/datasets/iwilldoit/emotions-sensor-data-set)