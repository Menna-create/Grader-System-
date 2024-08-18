# Grader-System-
Documentation for Python Code Grading System
Overview
This document provides a comprehensive overview of the Python code grading system, including design process, implementation steps, and a user guide. This system uses OpenAI's GPT-3.5-turbo model to evaluate Python code cells in Jupyter notebooks (.ipynb) and Python script files (.py) against a predefined rubric, assigning grades, and providing detailed feedback.
Design Process
1.	Objective: To create an automated grading system that evaluates Python code submissions based on correctness, efficiency, readability, code quality, and relevance to the question.

2.	Requirements:
o	Ability to read and process .py and .ipynb files.
o	Evaluate code cells based on a predefined rubric.
o	Provide detailed feedback for each cell.
o	Generate a summary table with grades and feedback.

3.	Tools and Libraries:
o	OpenAI API for GPT-3.5-turbo model.
o	nbformat and nbconvert for handling Jupyter notebooks.
o	tabulate for formatting the output as a table.
o	re for regular expression operations.
Implementation Steps
1.	Setup:
o	Install necessary libraries: openai, nbformat, nbconvert, and tabulate.
o	Obtain an OpenAI API key and set it in the script.

2.	Preprocessing Code:
o	Implement preprocess_code to perform initial checks and preprocessing on the code.

3.	Generating Feedback:
o	Implement generate_feedback to interact with the OpenAI API and get feedback for the code based on the rubric.

4.	Extracting Grades and Comments:
o	Implement extract_grades_and_comments to parse the feedback and extract scores and comments using regular expressions.

5.	Reading Files:
o	Implement read_python_file to read Python script files.
o	Implement read_notebook_file to read Jupyter notebook files and extract code and markdown cells.

6.	Main Function:
o	Implement the main function to handle user input, process files, generate feedback, and print the result table.

