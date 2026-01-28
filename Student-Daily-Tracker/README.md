# Student Daily Tracker System - Data Analytics project

This project is a **Student Daily Tracker System** analyzing students' daily academic activities and emotional states. Using data analytics techniques, the system extracts valuable insights from daily records including attendance, study hours, assignment and test scores, as well as mood tracking

---

## Dataset Description

The dataset `student_data.csv` contains daily records of students with the following columns:

- `Name` (string): Student's full name  
- `Date` (date): The date of the record (YYYY-MM-DD)  
- `Attendance (%)` (float): Percentage attendance on that day  
- `Study Hours` (float): Number of hours spent studying  
- `Assignment Score` (int): Score obtained in daily assignments  
- `Test Score` (int): Score obtained in tests/quizzes  
- `Mood` (string): Reported mood of the student (e.g., Happy, Neutral, Stressed, Tired)

---

## Project Workflow and Instructions Followed

### 1. Identifying and Sourcing Relevant Datasets
- Created and sourced a daily tracking dataset that covers academic and emotional parameters essential for student performance monitoring.

### 2. Cleaning and Handling Missing Values
- Loaded the dataset using pandas.
- Checked for missing or null values in all columns.
- Filled missing numerical values (`Attendance (%)`, `Study Hours`, `Assignment Score`, `Test Score`) with column means.
- For the categorical column `Mood`, missing values (if any) were filled with the mode (most frequent mood).

### 3. Feature Selection and Engineering
- Selected all relevant features affecting student performance.
- Converted `Date` column to datetime format for time-based analysis.
- Encoded categorical feature `Mood` into numerical values for correlation and analysis.

### 4. Ensuring Data Integrity and Consistency
- Checked for duplicates and removed if any.
- Verified correct data types for each column.
- Ensured consistency in data entries, especially for categorical moods.

### 5. Summary Statistics and Insights
- Computed summary statistics (mean, median, std deviation) for all numerical columns.
- Provided insights like average study hours, average attendance, typical assignment and test scores, and mood distributions.

### 6. Identifying Patterns, Trends, and Anomalies
- Used correlation matrix to understand relationships between attendance, study hours, scores, and mood.
- Identified any unusual values or outliers in study hours and scores using IQR.

### 7. Handling Outliers and Data Transformations
- Detected outliers in numerical columns using Interquartile Range (IQR) method.
- Applied transformations or capped outliers where necessary to avoid skewing analysis.

### 8. Initial Visual Representation of Key Findings
- Created visualizations such as:
  - Histograms for distribution of study hours and scores.
  - Boxplots for spotting outliers.
  - Scatterplots to show relationships between attendance, study hours, and scores.
  - Bar plots for mood frequency.
  - Time series plots for trends over dates.

---

## How to Use This Project

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Chandan-kumar10/Student-Daily-Tracker.git
   cd Student-Daily-Tracker


 2. Open Jupyter Notebook:
Open Student_Daily_Tracker.ipynb in Jupyter or VS Code with the Jupyter extension.

3. Install dependencies:

bash
Copy
Edit
pip install pandas numpy matplotlib seaborn


4. Run cells sequentially to execute:

Data loading and cleaning.
Feature engineering (date conversion, mood encoding).
Statistical summary and correlation analysis.
Outlier detection and handling.
Visualizations for insights.



#  Detailed Code Explanation Summary
Data Loading:
Read CSV with pd.read_csv() and converted Date column to datetime.

Handling Missing Values:
Numerical columns missing values filled with mean; categorical Mood filled with mode.

Feature Engineering:
Encoded Mood into numerical form for correlation analysis using pandas .map().

Data Integrity Checks:
Checked for duplicates, data types, and inconsistent entries.

Statistical Summary:
Used .describe() for numerical columns and .value_counts() for categorical moods.

Correlation Analysis:
Computed correlation matrix among numerical features including mood encoding.

Outlier Detection:
Applied IQR method on Study Hours, Assignment Score, and Test Score to find outliers.

Visualization:
Used matplotlib and seaborn for histograms, boxplots, scatterplots, bar plots, and time-series plots to present insights clearly.

# Tools and Technologies use. 
Python 3.x
pandas
Numpy
Matplotlib
Seaborn
Jupyter Notebook / VS Code

# conclusion
The Student Daily Tracker System offers a comprehensive analysis of students’ daily academic and emotional data, enabling identification of patterns and correlations that can inform better study habits and well-being monitoring.







