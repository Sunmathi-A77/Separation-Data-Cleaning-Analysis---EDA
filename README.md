# 📊 Separation Data Cleaning & Analysis – EDA

## 📌 Project Overview

This project focuses on data cleaning and exploratory data analysis (EDA) on a dataset containing separated names and IDs.
The goal is to clean raw data, perform basic analysis, and apply simple statistics to extract meaningful insights.

## 📂 Dataset Details

File Used: separated_names.csv 

Source - Kaggle (Link - https://drive.google.com/file/d/1wRJggH-4ROb2_1u8ohIEWFxwzrRsg3Bc/view?usp=sharing)

## Key Features:

id → Original field with ID and First Name combined.

ID → 5-digit unique identifier.

First_Name → Person’s first name.

## ⚙️ Steps Performed

## 🔹Basic Data Understanding (Pandas)

Loaded the dataset into a Pandas DataFrame

Displayed the first 10 rows

Checked shape, column names, and data types

Verified missing values and duplicates

Used .describe() to summarize:

ID (numeric statistics)

First_Name (categorical summary)

## 🔹Data Cleaning

Split raw ID column into:

ID → first 5 characters (converted to integer)

First_Name → remaining characters (string)

Stripped extra spaces from names

Standardized names into title case

Verified uniqueness of ID

## 🔹Exploratory Data Analysis (EDA)

Found the most common first name

Counted unique first names

Identified top 5 IDs (largest) and bottom 5 IDs (smallest)

Created a bar chart of top 10 most frequent first names

## 🔹Statistics

Computed mean, median, variance, and standard deviation of ID

Calculated probability that ID > 50000

Probability that a name starts with letter 'A'

Percentage of names with more than 5 letters

## 🔹Linear Algebra & NumPy

Converted ID column into a NumPy array

Created a random NumPy array for a new score column

Performed:

Vector addition and subtraction (ID ± score)

Dot product of ID and score

Matrix multiplication with:

Features = [ID, score]

Weights = [0.3, 0.7]

## 🔹Feature Engineering

Created:

Name_Length = number of characters in First_Name

Starts_With_Vowel = binary column (1 if starts with A/E/I/O/U)

High_ID = binary column (1 if ID > 50000)

Ranked names by length into 4 quartiles using qcut()

## 🔹SQL Simulation in Pandas

Selected rows where Starts_With_Vowel = 1 AND High_ID = 1

Retrieved top 10 IDs in descending order

Grouped by Starts_With_Vowel and counted rows

Sorted dataset by Name_Length (descending) and ID (ascending)

## 🔹Insights

Most frequent name identified

Average ID value computed

Trend check: correlation between ID size and name length

Determined which Name_Length quartile had the longest average IDs

## 📊 Visualizations & Insights

Bar charts of most frequent first names

<img width="554" height="494" alt="image" src="https://github.com/user-attachments/assets/bf94762d-f487-4117-85b1-07ed2bfa0a48" />

## 📌 Tech Stack

Python 🐍

Libraries: Pandas, NumPy, Matplotlib

## ✅ Results & Findings

Dataset successfully cleaned and structured

Found meaningful statistics and probabilities about IDs and names

Simulated SQL queries using Pandas operations

Extracted useful features (Name_Length, High_ID, Starts_With_Vowel) for analysis

Gained insights into relationships between IDs, names, and derived features
