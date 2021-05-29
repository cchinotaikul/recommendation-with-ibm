# Recommendation Engine for IBM Watson Studio Platform

This repository contains the files including raw data of articles and user interaction data of the [IBM Watson Studio](https://dataplatform.cloud.ibm.com/login) platform provided by IBM, and an exercise Jupyter Notebook which explores recommendation methods based on the data provided by Udacity, which looks at the rank-based, user-user-based, content-based, and matrix factorisation methods.

Created as part of my project for the Udacity Data Science Nanodegree course

This is the initial submission in order to meet the minimum requirement to pass the project. Extra optional tasks may be completed later.

## Installation

Data analysis created using Python 3.8.5 and Jupyter Notebook 6.1.5. Libraries used include:
- pandas (1.1.5)
- numpy (1.19.2)
- matplotlib (3.3.2)
- jupyterthemes (0.20.0)

## Project Motivation

In order to increase user engagement on contents on a platform, a robust recommendation engine is important, as it helps to lead users to contents that are relevant to their interests. In this project, we look at the main methods of recommendations including ranked-based, user-user-based, content-based, and matrix factorisation recommendations and how they can be implemented, as well as their benefits and limitations.

## File Descriptions

Files in this repository include:

<ul>
  <li>\data
    <ul>
      <li>articles_community.csv - CSV file with articles dataset</li>
      <li>user-item-interactions.csv - CSV file with user interactions dataset</li>
    </ul>
  </li>
  <li>Recommendations_with_IBM.ipynb - the main Jupyter Notebook file which reads in the data files, explore the data, and create recommendation engines based on the data</li>
  <li>Recommendations_with_IBM.html - html version of the Jupyter Notebook</li>
  <li>Testing files provided by Udacity for testing the functions in the Notebook include:
    <ul>
      <li>project_tests.py</li>
      <li>top_5.p</li>
      <li>top_10.p</li>
      <li>top_23.p</li>
      <li>user_item_matrix.p</li>
    </ul>
    </li>
</ul>

## Instructions

The Notebook can be viewed by opening the html file, or the Jupyter Notebook file can be run.

## Project Summary

The project is composed of the following key steps:

1. Exploratory Data Analysis - exploring the data files to gain insight on the key statistics of the data
2. Rank-Based Recommendations - Articles are ranked based on the number of interactions by users and the most popular articles would be recommended accordingly
3. User-User-Based Collaborative Filtering - By finding users who have had the most similar articles interactions to a user in question, we could recommend to the users articles that have been interacted with by similar users that they have not interacted with yet
4. Content-Based Recommendations - #TODO
5. Matrix Factorization - Using the matrix factorisation method, in this case the Singular Value Decomposition (SVD) method

We find that rank-based, user-user-based and matrix factorisation methods can be very useful in creating recommendations, but they are limited by the "cold start problem", where recommendations cannot be made for new users or articles as they do not have the required data to be input into the recommendation engine. This is where content-based recommendation would be helpful.

## Acknowledgement and Licensing

- Dataset provided by IBM
- Libraries' documentations
- Udacity course materials
- All files in this depository are free to use
