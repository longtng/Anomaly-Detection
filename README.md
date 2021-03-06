# Anomaly-Detection
The laboratory from Algorithmic Machine Learning Course at EURECOM

This repository included the Music Recommendation System Laboratory from the Algorithmic Machine Learning Course at EURECOM, which was conducted in a group with DANG Ngoc-Vien (Ngoc-Vien.Dang@eurecom.fr).

Furthermore, the Algorithmic Machine Learning Course was offered by Prof. Pietro Michiardi (http://www.eurecom.fr/~michiard/) at EURECOM. The details of the course can be retrieved in here https://github.com/DistributedSystemsGroup/Algorithmic-Machine-Learning

## Course Description
The goal of this course is mainly to offer data science projects to students to gain hands-on experience. It nicely merges the theoretical concepts students can learn in our courses on machine learning and statistical inference, and systems concepts we teach in distributed systems.

Notebooks require to address several challenges, that can be roughly classified in:
- Data preparation and cleaning
- Building descriptive statistics of the data
- Working on a selected algorithm, e.g., for building a statistical model
- Working on experimental validation

## The Laboratory Description
Anomaly detection (AD) refers to the process of detecting data points that do not conform with the rest of observations. Applications of anomaly detection include fraud and fault detection, surveillance, diagnosis, data cleanup, predictive maintenance.

When we talk about AD, we usually look at it as an unsupervised (or semi-supervised) task, where the concept of anomaly is often not well defined or, in the best case, just few samples are labeled as anomalous. In this challenge, you will look at AD from a different perspective!

The dataset you are going to work on consists of monitoring data generated by IT systems; such data is then processed by a monitoring system that executes some checks and detects a series of anomalies. This is a multi-label classification problem, where each check is a binary label corresponding to a specific type of anomaly. Your goal is to develop a machine learning model (or multiple ones) to accurately detect such anomalies.

This will also involve a mixture of data exploration, pre-processing, model selection, and performance evaluation. You will also be asked to try one or more rule learning models, and compare them with other ML models both in terms of predictive performances and interpretability. Interpreatibility is indeed a strong requirement especially in applications like AD where understanding the output of a model is as important as the output itself.

Please, bear in mind that the purpose of this challenge is not simply to find the best-performing model. You should rather make sure to understand the difficulties that come with this AD task.

### The Goals of this laboratory:
**Overview**

Beyond simply producing a well-performing model for making predictions, in this challenge we would like you to start developing your skills as a machine learning scientist. In this regard, your notebook should be structured in such a way as to explore the five following tasks that are expected to be carried out whenever undertaking such a project. The description below each aspect should serve as a guide for your work, but you are strongly encouraged to also explore alternative options and directions. Thinking outside the box will always be rewarded in these challenges.

**1. Data Exploration**

The first broad component of your notebook should enable you to familiarise yourselves with the given data, an outline of which is given at the end of this challenge specification. Among others, this section should investigate:

- Data cleaning
- Data visualisation;
- Computing descriptive statistics, e.g. correlation.
- etc.
Data exploration is also useful to identify eventual errors in the dataset: for example, some features may have values that are outside the allowed range of values. Ranges are specified in the dataset description.

**2. Data Pre-processing**

The previous step should give you a better understanding of which pre-processing is required for the data. This may include:
- Normalising and standardising the given data;
- Removing outliers;
- Carrying out feature selection, possibly using metrics derived from information theory;
- Handling missing information in the dataset;
- Augmenting the dataset with external information;
- Combining existing features.

**3. Model Selection**

At this point, you should have a good understanding of the dataset, and have an idea about the possible candidate models. For example, you may try a multi-label classification model to predict all classes at ones, or train different models, one for each label. In any case, it is important to justify your choices and make a comparison among the candidate models.

You are free to choose any model you want, but you should be aware about some factors which may influence your decision:

- What is the model's complexity?
- Is the model interpretable?
- Is the model able to handle imbalanced datasets?
- Is the model capable of handling both numerical and categorical data?
- Is the model able to handle missing values?
- Does the model return uncertainty estimates along with predictions?
An in-depth evaluation of competing models in view of this and other criteria will elevate the quality of your submission and earn you a higher grade. You may also try to build new labels by combining one or more labels (for example by doing an OR) and check if this impacts the performance of the model(s).

**4. Parameter Optimisation**

Irrespective of your choice, it is highly likely that your model will have one or more parameters that require tuning. There are several techniques for carrying out such a procedure, including cross-validation, Bayesian optimisation, and several others. As before, an analysis into which parameter tuning technique best suits your model is expected before proceeding with the optimisation of your model.

**5. Model Evaluation**

Some form of pre-evaluation will inevitably be required in the preceding sections in order to both select an appropriate model and configure its parameters appropriately. In this final section, you may evaluate other aspects of the model such as:
- Assessing the running time of your model;
- Determining whether some aspects can be parallelised;
- Training the model with smaller subsets of the data.
- etc.
