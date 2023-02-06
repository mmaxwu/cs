---
toc: true
layout: post
description: Providing an overview of the aspects and purpose of my part of the group's CPT plan
title: Individual Plan
categories: [Week 20, jupyter]
---

## Our Team Goal:
The end goal of the collegeboard create performance tasks is to challenge students to write a program and expertly explain a wide range aspects convered by the program in complexity management, purpose and functionality, and algorithm implementation. Due to this, we have begun a team project in hopes of practicing such skills. I personally work on one small program of our entire project, but within this sub program still contains all of the required collegeboard aspects.

## Video:
I will first play a round of snake, then go through all our features. The first feature is the leaderboard, and I will show the score saving into the leaderboard, and replacing a score on there. Then I will play the snake game again, getting a better score this time, I will show the leaderboard updating to my new score, and also showing the history log for that user. 

## My Portion:
My portion of the project is logging the history of the 5 most recent scores of every user. My part of the program will be connected with the DB because the history will be persistent data. 


## Row 1 - Purpose and Function
In my write-up, I will first review the program’s purpose, function and inputs, which is to provide the users with a fun and interactive experience that they can revisit and compete with others

## Row 2  - Data Abstraction
The first code section displays the "json_ready" list in the "ScoreListAPI" class in the "score.py" file located in the "api" folder. The second code section, located directly below the list, displays all code below the line "return jsonify(json_ready)". This list holds all the data for the entered scores and profile information.

## Row 3 - Managing Complexity
Manages complexity by generating all the history into a table

## Row 4 - Procedural Abstraction 
1. Create a database table to store the user's information, including their username, score, and date of the score.

2. Write a function that allows a user to submit their score. This function should take in the user's username and score as input, and store this information in the database table.

3. Write a function that retrieves a user's score history, which should retrieve all of the scores for a given username from the database table.


## Row 5 - Algorithm Implementation
I will add the code segment "def initScores()" in the model folder of scores.py. This function sets up a test database and tables, adds users with specified parameters to a list, and uses a for loop to input the data into the table. It also includes try and except statements.

## Row 6 - Testing 
Calls: Input the data into the table
Conditions: create() function used for creating new data
Result: Logs all the username scores into the table


<mark>We haven't automated database yet, so the data will be manually inputted by us for testing reasons</mark>

