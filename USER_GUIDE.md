# Introduction
This program is a grade calculator. You input the total number of points you can get in a class, and then you input how many points you've actually earned. The result is your final grade.

## Getting Started
### How to Build
Using g++ (Linux / macOS / WSL / MinGW):

    g++ -std=c++17 main.cpp Greeting.cpp -o GradeCalculator

### How to Run
    ./GradeCalculator        # macOS / Linux
    GradeCalculator.exe      # Windows

## Step-by-Step Walkthrough
You will be given a number of prompts that require specific inputs. Here they are explained in order:
1. You will be asked to input your total number of points. The input must be a positive whole number.
2. You will then be prompted to input the minimum points required for recieving an 'A', 'B', 'C', or 'D'. The input for these must be a positive decimal number.
3. Next, you will be asked to provide entries for your assignments. You will first input a positive decimal number for how many points you got for that assignment, and then you will be asked to provide a name for that assignment as a string of text. It will keep asking you for more and more assignments unless you submit a negative number for the assignment score. Once you submit a negative number for the assignment score.
4. After all your inputs, Your results should show up at the very end!

## Sentinel Value Reminder
Don't forget that entering a negative number as an assignment score will end the looping prompts for assignments! Don't worry, the negative number will not be submitted as a score itself.

## Sample Session
    Good Evening!

    Welcome to Your Grade Calculator!

    Grading Scheme Setup
    ====================
    Please input the Total Points Possible: 100
    Please input the Minimum Points for a 'A': 90
    Please input the Minimum Points for a 'B': 80
    Please input the Minimum Points for a 'C': 70
    Please input the Minimum Points for a 'D': 60

    The Grading Scheme You Input
    ============================
    Total Points Possible in the Course: 100
    Points needed for an 'A': 90
    Points needed for a 'B': 80
    Points needed for a 'C': 70
    Points needed for a 'D': 60

    Grade Calculation
    You will be prompted to input scores for all assignments.
    (Input a negative number to cease input and calculate letter grade.)

    Please input the points earned for Assignment 1: 50
    Please input the name for Assignment 1: exam 1
    Please input the points earned for Assignment 2: 25
    Please input the name for Assignment 2: homework 1
    Please input the points earned for Assignment 3: 15
    Please input the name for Assignment 3: homework 2
    Please input the points earned for Assignment 4: -1

    Assignments Sorted by Score (Highest to Lowest)
    ===============================================
    exam 1: 50 points
    homework 1: 25 points
    homework 2: 15 points


    Final Results
    Total Points Earned: 90
    Total Points Possible: 100
    Total Percentage: 90%
    Final Letter Grade: A

## Understanding Your Results
The results of your program should tell you the points that you earned and the total points you could have gotten. Next, it'll show you your percentage grade in the class. Finally, you'll see your resulting letter grade. 

## Troubleshooting
There are some common mistakes or problems you may run into. Here are the common causes:
- Entering a number or string of text where the program isn't expecting one. Check the step-by-step walkthrough in this file to see what the program expects!
- Getting stuck in the assignment input section. Remember to enter a negative number as an assignment score after you're done inputting your assignments!