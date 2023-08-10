# Eat, Safe, Love - nosql-challenge

Python, mongoimport, PyMongo, Pandas

## Background
The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## Setup and Update the database
This step can be found within the NoSQL_setup jupyter notebook. The data provided in the Resources folder was imported on git bash using `mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json`. A new resturant was added to be included in the analysis phase and some data cleaning was done.

## Exploratory Analysis
This step can be found within the NoSQL_analysis jupyter notebook. the following questions were to explore the database, find the answers, and provided to the magazine editors:

### 1. Which establishments have a hygiene score equal to 20? </br>
  There are 41 establishments with the hygiene score of 20. They are saved in the DataFrame `hygiene_20`

### 2. Which establishments in London have a RatingValue greater than or equal to 4 </br>
  There are 33 establishments in London with the rating value of 4 or higher. They are saved in the DataFrame `rating_gte4`

### 3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
  The top 5 establishments meeting the requirements are: `Volunteer, Plumstead Manor Nursery, Lumbini Grocery Ltd T/A Al-Iman, Iceland and Howe and Co Fish and Chips - Van 17`. They are saved in the DataFrame `top_5_near_penang`

### 4. How many establishments in each Local Authority area have a hygiene score of 0?
  55 Local Authorities returned a count for a hygiene score of 0 with `Thanet` at number one with a count of `1130`. The results are saved in the Dataframe `hygiene_local_authority`
  
  ![image](https://github.com/nicduffee/nosql-challenge/assets/91498217/0ea663fb-afff-4ff8-8720-6f3a02debc03)
