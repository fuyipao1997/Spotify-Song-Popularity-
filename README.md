# Spotify-Song-Popularity-Prediction
## <b> 1. Project Motivation</b>
Nowadays, music has become an integral to our life, and Spotify plays an important role. As a global leader in the streaming music sector, Spotify has over 456 million monthly active users, including 195 million paying subscribers. For most people, it has become part of their daily routine. However, this outbreak has increased our music listening activities.
Thus, we aim to understand the features that popular songs have in common. Moreover, we’re interested in knowing if a song's artist, the genre of songs and the musical features like energy, loudness and danceability among others can help distinguish hit and non-hit songs. Our project goal is to evaluate machine learning models from Python to predict Spotify song popularity and identify what makes a song popular.
## <b> 2. Data Source</b>
The dataset for our project is based on the following link from Kaggle:
https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset
## <b> 3. Report Summary</b>
Our team aims to evaluate machine learning models to predict Spotify song popularity and identify what makes a song popular. We performed data cleaning, exploration of the dataset, and build ML models in Python.

In phase one, we implemented exploratory data analysis. For better data usage, we changed the data types, deleted one missing value, and dealt with outliers in the "tempo" column. We then did a general EDA and got a high level understanding of the dataset. Most popular songs(defined by popularity over 70) shared the traits of low acoustics, higher danceability, higher energy, and tempos between 90-120. The correlation matrix shows some strong relationships between features.

With a basic understanding of the dataset, our team moved on to phase two: song popularity prediction. To predict precise popularity scores, we started with Linear Regression. However, it turned out that linear regression did not fit our data well because of the extremely low R-square even after considering interactions. 

Our team wasn’t stopped by the challenge. We decided to conduct classifier models by labeling the song popularity scores into "Popular", "Somewhat Popular", and "Unpopular". Four models, Random Forest, Decision Tree, KNN, and Logistic regression, were trained, and the Decision Tree and Logistic Regression showed nearly 0.55 accuracy. 

We were still trying to optimize our model with Grid Search to tune our hyperparameters and also with bagging and boosting ensemble methods, which raised the accuracy by 10%. In the end, we realized that class imbalance in our dataset(with a low proportion of “very popular” tracks) could be handled by over/under sampling methods. At the end of the day, our Logistic Regression model reached an accuracy of over 0.71.

Our biggest challenge throughout the project is improving the model performance with trial and error in limited time and resources. Tunning the better-performing model and the progress from 0.4 to 0.7 did enlighten us. We gained precious experience in this project.
