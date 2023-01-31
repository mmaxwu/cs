---
toc: true
layout: post
description: Providing an overview of the aspects and purpose of my part of the group's CPT plan
categories: [Week 20, jupyter]
---

## Our Team Goal:
The end goal of the collegeboard create performance tasks is to challenge students to write a program and expertly explain a wide range aspects convered by the program in complexity management, purpose and functionality, and algorithm implementation. Due to this, we have begun a team project in hopes of practicing such skills. I personally work on one small program of our entire project, but within this sub program still contains all of the required collegeboard aspects.

## Video:
I will first play a round of snake, then go through all our features. The first feature is the leaderboard, and I will show the score saving into the leaderboard, and replacing a score on there. Then I will play the snake game again, getting a better score this time, I will show the leaderboard updating to my new score, and also showing the history log for that user. 

## My Portion:
My portion of the project is logging the history of the 5 most recent scores of every user. My part of the program will be connected with Evan's leaderboard, because the leaderboard will use the data from my history, to refresh his score. 


## Row 1:
In my write-up, I will first reivew the program’s purpose, function and inputs, which is to provide the users with a fun and interactive experience that they can revisit and compete with others

## Row 2: 
The first code section displays the "json_ready" list in the "ScoreListAPI" class in the "score.py" file located in the "api" folder. The second code section, located directly below the list, displays all code below the line "return jsonify(json_ready)". This list holds all the data for the entered scores and profile information.

## Row 3
Manages complexity by generating all the history into a single list

## Row 4
The functions in the code lack proper parameters. I would start with the create(self) function in the model folder of scores.py. I will demonstrate its usage in the api folder of score.py on line 37 and in the if user: statement. This function is important because it converts the data entered into the table into a JSON format.

## Row 5
I will add the code segment "def initScores()" in the model folder of scores.py. This function sets up a test database and tables, adds users with specified parameters to a list, and uses a for loop to input the data into the table. It also includes try and except statements.

## Row 6
Calls: Input the data into the table
Conditions: create() function used for creating new data, delete() function to delete the existing data.
Result: Logs all the username scores into the table

