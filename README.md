# Shakespeare_Plays
The datafile is stored inside the 'Notebook' directory. The steps are written here. However, the classification has been done inside the notebook.

STEP_1:
Import the csv dataset and load it as a pandas dataframe

STEP_2: DATA CLEANINING/PREPROCESSING
Remove all the records for which either of the PlayerLinenumber, ActSceneLine or Player is NaN

STEP_3: FEATURE ENGINEERING
Task: To classify the plays into categories of 16th Century Play or 17th Century Play.
Step 3.1: Get all the unique values of the Plays (from the 'Play' Column)
Step 3.2: Create a new custom feature called 'Year' using the function create_year_of_play() and applying it on the 'Play' feature/column using apply() method.
Step 3.3: Write a function period_of_play() to classify the plays into categories of four periods of Shakespeares' plays. This function is applied on the newly developed custom feature 'Year'.
Step 3.4: Write a function century_of_play() to classify the plays into categories of century. This function is applied on the newly developed custom feature 'Year'.

STEP_4: Get Data insights after feature engineering
4.1. Plays per year¶
4.2. Plays per period of writing
4.3. Players/Actors/Characters per play¶
4.4. Characters in most number of scenes, ordered by period of writing

CLASSIFICATION ON SAME DATA
Applying Classification Techniques on the same data but loaded into different Data Frame

Accuracy Results
Naive Bayes = 30.9%
Logistic Regression = 55.55%
Random Forest = 35.52%
