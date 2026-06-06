Task 1: Data Cleaning & Preprocessing - Titanic Dataset

Hi there! My name is [Your Name], and this is my first data science project, completed as part of my internship at Synent Technologies.

So, What is this all about?

Ever opened a spreadsheet and found tons of missing entries, weird abbreviations, and jumbled data? That's what real-world data often looks like.

The Titanic dataset, which contained 891 passenger records, was a prime example of this:
- Missing values in the 'age' column
- Unintuitive column names
- Random holes in the data
- Unorganized data types

My task was to clean this data and get it ready for analysis.

What I've Done:

Step 1: Exploratory Data Analysis
My first step was to open the dataset and take a look. "Wow, this is quite messy!" I thought.

I discovered that there were:
- 891 rows (representing individual passengers)
- 12 columns (containing passenger details)
- Several missing values in the 'age' column
- Two missing values in the 'embarked' column

Step 2: Handle Missing Values
Since the 'age' column had a significant number of missing values (177 passengers), I decided to fill them with the average age (29.7 years) of the existing passengers.

The two missing values in the 'embarked' column were filled with the most frequent port of embarkation, which was Southampton.

The 'cabin' column was almost entirely empty (77% missing data), so I simply removed it as it was not useful.

Step 3: Remove Duplicates
I checked for any duplicate passenger entries in the dataset. Fortunately, there were none!

Step 4: Fix Data Types
I noticed that some of the columns with numerical data were stored as text. I converted them to the correct data type to enable numerical operations. This included:
- Survived (0 or 1)
- Pclass (1, 2, or 3)
- Sex (Male or Female)

Step 5: Rename Columns
I renamed some columns to be more descriptive and user-friendly. For example:
- 'PassengerId' to 'Passenger_ID'
- 'Pclass' to 'Passenger_Class'
- 'SibSp' to 'Siblings_Spouses'
- 'Parch' to 'Parents_Children'

Step 6: Save Clean Data
Finally, I exported the cleaned dataset as 'titanic_cleaned.csv'.

Interesting Findings:

After cleaning the data, I found a few interesting things:

- There were a total of 891 passengers on board.
- Sadly, only 342 passengers survived, which is 38% of the total.
- 62% of the passengers (549 individuals) did not survive.
- The average age of the passengers was 29.7 years.
- The majority of passengers embarked from Southampton.
- There was a significantly higher survival rate among women compared to men (the "women and children first" rule appears to have been followed!).

How to Use:

1. Download the notebook.
2. Place the 'Titanic.csv' file in the same directory.
3. Open and run the notebook.
4. Watch the data cleaning magic unfold!

What's Included:

Project Folder:
  - titanic.ipynb (My notebook)
  - Titanic.csv (Original, raw data)
  - titanic_cleaned.csv (Cleaned and ready-to-use data)
  - missingvaluesheatmap.png (A visual representation of missing values)

What I Learned:

1. Data cleaning is crucial and takes a lot of time – often the biggest part of a data science project.
2. Thoroughly understanding your data before you start is essential.
3. There's no single solution for handling missing data; the approach depends on the column.
4. Visualizing the data, especially missing values with a heatmap, is incredibly helpful.
5. Renaming columns makes your code and the final dataset much easier to understand and work with.

Technologies Used:

- Python
- Pandas (for data manipulation)
- NumPy (for numerical operations)
- Matplotlib (for basic plotting)
- Seaborn (for more advanced and aesthetically pleasing plots)

By Raj Javiya
Internship at Synent Technologies 2026
