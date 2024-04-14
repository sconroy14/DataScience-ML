# Predicting and Understanding Viewer Engagement with Educational Videos

## Introduction
With the increasing popularity of online educational experiences, the importance of online lectures and educational videos is growing. This assignment focuses on predicting viewer engagement with educational videos, which is crucial for understanding learners' preferences and improving learning outcomes.

## About the Prediction Problem
The goal of this assignment is to predict how engaging an educational video is likely to be for viewers based on various features extracted from the video's transcript, audio track, hosting site, and other sources. The target variable is whether the median percentage of the video watched across all viewers was at least 30%.

## About the Dataset
The dataset consists of training and test datasets of educational video features extracted from the VLE Dataset by researcher Sahan Bulathwela at University College London. Each row in the dataset represents a single educational video and includes features such as title word count, document entropy, freshness, easiness, fraction of stopword presence, speaker speed, and silent period rate. The target variable in the training set is 'engagement'.

**Data Fields**:
- title_word_count: Number of words in the title of the video.
- document_entropy: Score indicating how varied the topics are covered in the video, based on the transcript.
- freshness: Number of days elapsed between 01/01/1970 and the lecture published date.
- easiness: Text difficulty measure applied to the transcript.
- fraction_stopword_presence: Fraction of all words that are stopwords in the video lecture transcript.
- speaker_speed: Average speaking rate in words per minute of the presenter in the video.
- silent_period_rate: Fraction of time in the lecture video that is silence (no speaking).

**Evaluation Metric**: Area Under the ROC Curve (AUC)

## Evaluation
The predictions will be evaluated based on the AUC score computed for the classifier. A model with an AUC of at least 0.8 passes the assignment.

