# Classification in Python
In this guide, we provide a tutorial for your team to perform classification on your data. In particular, we will utilize a widely-used Python library called "scikit-learn", and we will demonstrate the detailed steps by walking through a dataset on predicting if a person is less/more likely to get a heart attack. In the following sections, we will introduce you to classification and a description of the dataset.

## Python
Python is a programming language that is effectively used to conduct data analysis - it's also easy for beginners to pick up. It contains more than 137,000 libraries which are built-in and can be directly imported to use. The library used in this tutorial, scikit-learn, provides simple and efficient tools for predictive data analysis, including classification, regression, clustering and dimensionality reduction.

Please refer to [this link](https://github.com/nmcdowell00/python_for_the_datajam#jupytrlab-and-andaconda) for downloading and setting up Jupyter Notebook.

Once you have set up a notebook and created a code block, you can hit the small triangular button on the left-hand side of the block to run your code (like below).
[![](https://cdn.glitch.global/91d27b43-3628-403c-9755-b2f6c8f75fbf/button.jpg?v=1671242043616)](http://https://cdn.glitch.global/91d27b43-3628-403c-9755-b2f6c8f75fbf/button.jpg?v=1671242043616)

## Classification and Classifiers
### What is Classification?
Suppose you have a dataset about flowers, including:
- variables: the length of a petal, color, and how strong the scent is
- corresponding labels: what kind this flower is (lily, rose, or sunflower)

Classification is to categorize data into different groups by variable values. In this example, the goal of classification is to tell whether a flower is a lily, rose, or sunflower based on the petal length, color, and scent of this flower.

### What is a Classifier?
A classifier is an algorithm[1] that allows you to perform classification, i.e., categorize data into groups. One of the most common examples is an email classifier that scans emails to filter them by the labels of *Spam* or *Not Spam*. 

[1]: If you are wondering what an algorithm is - it is a sequence of instructions to solve a problem. It is everywhere in our lives. One example is instructions on how to bake a cake:
-- Preheat the oven
-- Mix together the ingredients to make the batter
-- Pour the batter into the pan
-- Put the pan in the oven
-- Take the pan out of the oven

With a classifier in hand, we can apply it to new data to predict a category for it. 

## Demo Dataset
In our demo data, we are interested in whether a person is less/more likely to get a heart attack. 

We have the following ten variables:
- the age of a person
- the gender of a person (1: Male, 0: Female)
- chest pain type
- resting blood pressure
- cholestoral in mg/dl
- if fasting blood sugar > 120 mg/dl (1: yes, 0: no)
- resting electrocardiographic results
- maximum heart rate achieved
- if exercise induced angina (1: yes, 0: no)
- previous heart attack peak

Each data entry containing values for these variables has a corresponding "output" label. If the label is 1, the person is very likely to get a heart attack, while if the label is 0, the person is less likely to get a heart attack. Please refer to this tutorial to see how to build a common type of classifier, Logistic Regression, to classify the data using scikit-learn.
