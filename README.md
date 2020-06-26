# Toxic Comment Classification
### Pujan Malavia
![jigsaw](https://user-images.githubusercontent.com/19572673/85205534-e22dd500-b2e9-11ea-866f-a23a9174ed8a.jpg)

### Link to Dataset: 

https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data

### Abstract:

Discussing things you care about can be difficult. The threat of abuse and harassment online means that many people stop expressing themselves and give up on seeking different opinions. Platforms struggle to effectively facilitate conversations, leading many communities to limit or completely shut down user comments.

The Conversation AI team, a research initiative founded by Jigsaw and Google (both a part of Alphabet) are working on tools to help improve online conversation. One area of focus is the study of negative online behaviors, like toxic comments (i.e. comments that are rude, disrespectful or otherwise likely to make someone leave a discussion). So far they’ve built a range of publicly available models served through the Perspective API, including toxicity. But the current models still make errors, and they don’t allow users to select which types of toxicity they’re interested in finding (e.g. some platforms may be fine with profanity, but not with other types of toxic content).

In this competition, you’re challenged to build a multi-headed model that’s capable of detecting different types of of toxicity like threats, obscenity, insults, and identity-based hate better than Perspective’s current models. You’ll be using a dataset of comments from Wikipedia’s talk page edits. Improvements to the current model will hopefully help online discussion become more productive and respectful.

Disclaimer: the dataset for this competition contains text that may be considered profane, vulgar, or offensive.

### Industry:

Internet, Technology

### Company Information:
Jigsaw is a team of engineers, researchers and geopolitical experts who build products to support free expression and access to information, especially in repressive societies. We focus on the problems faced by people who live in unstable, isolated, or oppressive environments, including the billions of people who are coming online for the first time.

https://www.linkedin.com/company/jigsaw-google

https://jigsaw.google.com/

### Initial Dataset(s):
train.csv - the training set, contains comments with their binary labels

test.csv - the test set, you must predict the toxicity probabilities for these comments. To deter hand labeling, the test set contains some comments which are not included in scoring.

sample_submission.csv - a sample submission file in the correct format

test_labels.csv - labels for the test data; value of -1 indicates it was not used for scoring; (Note: file added after competition close!)

### Use Case:
Build a model to predict a probability for each of the six possible types of comment toxicity (toxic, severetoxic, obscene, threat, insult, identity, and hate)

### Tool:
Python (Jupyter Notebook)

### Data:
You are provided with a large number of Wikipedia comments which have been labeled by human raters for toxic behavior.

### Data Fields:
id: respective unique ID

comment_text: Unstructured text jargon

The types of toxicity are:

toxic

severe_toxic

obscene

threat

insult

identity_hate

### Data Visualization

Python (Jupyter Notebook) Visualizations

https://github.com/pm831/Toxic_Comment_Classification/blob/master/Toxic_Comment_Classification.ipynb

Comment Text Distribution

![output_22_1](https://user-images.githubusercontent.com/19572673/85776545-d2016580-b6ee-11ea-84e1-1e913763cc11.png)

Labels Frequency Plot (toxic, severe_toxic, obscene, threat, insult, identity_hate)

![output_24_1](https://user-images.githubusercontent.com/19572673/85776549-d2016580-b6ee-11ea-8545-48da1594c232.png)

Visualizing F1 score results through box-plot.

![output_36_0](https://user-images.githubusercontent.com/19572673/85776551-d299fc00-b6ee-11ea-88cd-8c11d9358b03.png)

Code to create bar graph of F1 and Recall across each label for Multinomial Naive Bayes

![output_37_2](https://user-images.githubusercontent.com/19572673/85776554-d299fc00-b6ee-11ea-8947-181f8d94163d.png)

Code to create bar graph of F1 and Recall across each label for Logistic regression

![output_38_2](https://user-images.githubusercontent.com/19572673/85776555-d299fc00-b6ee-11ea-882d-ddaddcdc78d1.png)

Code to create bar graph of F1 and Recall across each label for Linear SVC

![output_39_2](https://user-images.githubusercontent.com/19572673/85776557-d3329280-b6ee-11ea-90de-cfd67d4f0514.png)

Confusion Matrix: Multinomial Naive Bayes

![output_42_1](https://user-images.githubusercontent.com/19572673/85776559-d3329280-b6ee-11ea-8b69-0bd7330a8bc7.png)

Confusion Matrix: Logistic Regression

![output_42_3](https://user-images.githubusercontent.com/19572673/85776561-d3329280-b6ee-11ea-8821-fdce94e24abc.png)

Confusion Matrix: Linear SVC

![output_42_5](https://user-images.githubusercontent.com/19572673/85776564-d3329280-b6ee-11ea-914a-6bedd5ef973e.png)

Word Cloud

![output_58_0](https://user-images.githubusercontent.com/19572673/85776566-d3329280-b6ee-11ea-99be-446a09ea3ae3.png)

Learning Curves (Linear SVC) for TOXIC

![output_62_1](https://user-images.githubusercontent.com/19572673/85776569-d3cb2900-b6ee-11ea-8815-5b5600aef151.png)
