# Netflix-data-science-project
![<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/fac526a2-1ff6-4d90-9139-bcaed9b5524d" />
]


**Project Overview**

This project aimed to build a data science workflow in Google Colab using Python to analyze a dataset of movies and TV shows, with the goal of predicting IMDb scores. The process involved loading data, exploring its characteristics, cleaning it, creating new relevant features, building a machine learning model, and evaluating its performance.

**Data Analysis Key Findings**

Data Loading and Initial Look: We successfully loaded the dataset and got an initial look at the information it contains, such as release year, duration (runtime), and viewer ratings (IMDb score). We also saw whether an entry was a movie or a TV show and its age certification.
Understanding the Data (EDA): Our initial exploration showed that some data points were missing, particularly for age certifications. We also observed that most titles were released in recent years, runtimes often fall between 90 and 100 minutes, and IMDb scores tend to be on the higher side. We didn't find a simple straight-line relationship between release year and IMDb score. There are more movies than TV shows in the dataset, and age certifications are quite varied, with a large portion uncategorized.
Cleaning and Preparing Data: To make the data usable for our model, we handled the missing information. We filled in missing viewer counts and marked missing age certifications as 'Unknown'. We also added the length of the title as a potential feature. We then converted categories like 'type' and 'age certification' into a format the model could understand.
Building a Predictive Model: We chose a Random Forest Regressor model to predict IMDb scores. This type of model is good at finding complex patterns. We trained it on a portion of our data and tested its predictions on the rest.
Model Performance: We evaluated our model's ability to predict IMDb scores using metrics like Mean Squared Error (MSE) and R-squared (R2). The MSE of approximately 1.08 tells us the average squared difference between our model's predictions and the actual IMDb scores – a lower number is better. The R-squared score of approximately 0.21 means that about 21% of the variation in IMDb scores can be explained by the features our model used.
