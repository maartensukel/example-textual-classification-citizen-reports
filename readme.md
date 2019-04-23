# A simple textual classifier for Dutch citizen service requests

In many cities in the world local governments offer a service where citizens can make requests, for example to make a complaint about garbage on the street or to report nuisance. These reports are made by phone or trough a webform, by writing a text and selecting a category. The selection of a category can be done by using supervised machine learning on historical service requests. The city of Amsterdam uses this method to detect the class of an report and route it to the correct department. In this repository is the python code that can be used to create such a classifier.

The classification is done by using a TF-IDF (Term Freuqency - Inversed document frequency) as representation for the text and a logistic regression to classify the text. Optimal hyperparameters for the dataset are found using a gridsearch.

An example subset of data of dutch citizen reports is added for demonstration purposes. The original data used is not publicly available due to privacy concerns.

A live demo of a textual classification of Dutch service requets can be seen at http://ec2-54-171-141-211.eu-west-1.compute.amazonaws.com/

A medium story describing the creation of the classifier can be seen at https://medium.com/maarten-sukel/how-to-use-machine-learning-for-the-classification-of-citizen-service-requests-b71159a85f36