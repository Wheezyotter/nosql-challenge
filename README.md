# nosql-challenge
NoSQL-challange is an exercise to practice using mongoDB databases and pymongo to clean and analyze data. 

To practice these skills, the scripts aim to read data from establishments across the UK based on provided sample data found in the Resources folder and query specific information from it. NoSQL_setup.ipynb reads and cleans the data while noSQL_analysis.ipynb analyzes the data. 

### Part 1: NoSQL_setup.ipynb
---
Data is imported into mongoDb using the following in the console: 

    mongoimport --type json  -d uk_food -c establishments --drop --jsonArray establishments.json

In this script the data is imported using pymongo and updated to include and new restaurant 'Penang Flavours'. The data types for "RatingValue" and "Geocode" are then updated for the entire database. 

### Part 2: NoSQL_analysis.ipynb 
---
In this script pymongo is used to answer four questions and store the queried results in a pandas dataframe.

1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a "RatingValue" greater than or equal to 4?
3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

---
Script was made for UCB Data Analytics Challenge 12

Author - Jacob Pohs