# Student Performance & Class Standing System

A simple console-based academic tracking system written in Python.
It supports **Admin** and **Student** modes for recording quiz scores, module scores, viewing detailed score histories, and calculating overall class standing grades.

Features

Main Menu

* Admin Mode — Allows recording of scores and viewing class standing
* Student Mode — Allows students to check their own quiz/module scores and grades
* Exit System — Closes the application

Admin Menu

1. Record Quiz Scores (with validation and multi-entry support)
2. Record Module Scores (with validation and multi-entry support)
3. View Class Standing Grade
4. Logout

Student Menu

1. View Quiz Scores
2. View Module Scores
3. View Class Standing Grade
4. Exit

How to Run

1. Make sure you have Python 3 installed.
2. Save the code as a `.py` file (e.g. `grading_system.py`).
3. Run it:

```bash
python grading_system.py

or

python3 grading_system.py****

Key Behaviors

1. Score Validation: Ensures quiz and module inputs are numeric, prevents scores higher than the overall score, and blocks zero overall values.
2. Interactive Exit ('B' Key): Allows admins to easily exit the scoring loop at any time by entering 'B'.
3. Data Aggregation: Automatically computes accumulated earned scores versus overall points for both quizzes and modules.
4. Role-Based Access: Dedicated interfaces for administrators to input data and students to view their individual progress.

Project Structure (Single File)
1. All data is managed in memory using nested Python data structures:
2. quiz_list & module_list — Stores recorded score entries per student and subject (e.g., "15/20")
3. quiz_earned & quiz_overal — Tracks accumulated total quiz points4 
4. module_earned & module_overall — Tracks accumulated total module points
5. choose_students() & choose_subjects() — Helper functions for navigation selection
6. class_standing() — Function for calculating and displaying final grade summaries

No external libraries or databases are required — standard Python execution only.

Notes

1. Data is not persisted. All entered scores reset once the program is closed.
2. This is a console / terminal application (text-based interface).
3. Designed for simple classroom / project demonstration purposes.

Author

Created by TechLarpers.
Feel free to improve it (add file saving, database, GUI, etc.).
