# Medicine-Recommendation-System
A content-based medicine recommendation system built using Python, TF-IDF, and cosine similarity.
# Features

Recommends the top 5 medicines for a disease/reason.

Case-insensitive input: works regardless of capitalization.

Uses TF-IDF vectorization on the disease description to compute similarity.

Interactive input loop to test multiple queries.

Easy to extend with new datasets.

# Dataset

The system uses a CSV dataset with the following columns:

Column Name	Description,
Drug_Name	Name of the medicine/drug,
Reason	Disease or reason for taking the medicine,
Description	Description of the disease or symptoms.

# How It Works

Loads the medicine dataset with Drug_Name, Reason, and Description.

Preprocesses the data:

Drops missing values

Creates a lowercase version of the Reason column for case-insensitive matching.

Converts the Description column into TF-IDF vectors.

Computes cosine similarity between all diseases/reasons.

For a given input disease/reason, finds the most similar diseases and recommends their medicines.

Interactive loop allows users to input multiple queries.
