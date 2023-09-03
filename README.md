# nosql-challenge

# Eat, Safe, Love 
# Overview
The purpose of this analysis is to assist journalists and food critics in deciding where to focus their research based on data insights. A significant focus of the analysis revolves around food hygiene ratings data. The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles. 

# Database Setup
To run the analysis, follow these instructions:

Import the data from the establishments.json file using the following terminal command:
mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

# Libraries and Tools Used
We utilized the following libraries and tools in this analysis:

+ PyMongo
+ Pretty Print (pprint)
+ Pandas (pd)

# Database Modifications
In this part of the analysis:

+ A new restaurant named "Panang Flavours" was added to the database.
+ Searches were conducted around the new restaurant based on latitude, longitude, and hygiene scores.
+ Documents related to "Dover" were removed from the collection.

# Key Analysis Findings
In London, 33 establishments have a RatingValue of 4 or higher. (See below for a sample DataFrame)
The top 5 establishments, sorted by the lowest hygiene score, near the new restaurant "Panang Flavours" were identified.
![image](https://github.com/yakopeca/nosql-challenge/assets/132225987/6d05b576-5d41-4e08-b18e-a7188043c1dd)


After thorough research, here are the counts of establishments with a Hygiene score of 0 in each Local Authority. The following information could be used when deciding where to stay when visiting the UK. 

![image](https://github.com/yakopeca/nosql-challenge/assets/132225987/26ef5242-10f3-4734-a2f5-bfc7060045c5)

# Usefulness for "Eat, Safe, Love"
These analysis results serve as foundational grounds for food critics and journalists, helping them choose which restaurants to feature in their articles. This data analysis is valuable for future researchers interested in food, restaurants, and rating values. It simplifies the process of choosing your next meal by providing valuable insights into food hygiene ratings.
