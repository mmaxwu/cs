---
toc: true
layout: post
description: 
title: Binary Math and Truth Tables HACKS
---

## Binary Math
### Conversion Exercises 

Convert the following numbers to decimal notation:
The binary number 111.: **7**
The binary number 1011.: **11**
The binary number 10111011.: **187**

### BINARY MATH HACKS

DIFFERENCES OF BINARY MATH NUMBERS:

{% include binarymath.html %}


### Hacks


**Question**: How do you think we should find the difference of two binary numbers? The product? The quotient? What rules need to be followed for those operations? Look into all of this on the Internet and note down important information you find (0.45) 

**To find the difference of two binary numbers, we need to subtract the subtrahend (the number being subtracted) from the minuend (the number being subtracted from). To do this, we can find the 2's complement of the subtrahend and add it to the minuend. If there is a carry after the addition, we need to discard it to get the correct answer.**



Based on what you find online, fill out the tables below for subtracting, multiplying, and dividing binary numbers (0.45):


**Subtracting Binary Numbers Rules**

|---------|---------|---------|---------|
| **1-1** | **1-0** | **0-1** | **0-0** |
|    0     |     1    |     1    |     0    |


**Multiplying Binary Numbers Rules**


|---------|---------|---------|---------|
| **1x1** | **1x0** | **0x1** | **0x0** |
|    1     |     0    |    0     |    0     |


**Dividing Binary Numbers Rules**

|---------|---------|
| **1/1** | **0/1** |
|     1    |    0    |        


Choose ONE (0.9 for doing one):

- Create buttons similar to the ones above that allow you to **subtract** binary numbers and returns the desired result in both binary and decimal

In the above button, I was able to create a button that **subtracts** binary numbers and returns that desired result in both binary and decimal.

## Binary Logic
![]({{site.baseurl}}/images/binarylogic.png)
