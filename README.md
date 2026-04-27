 Project Overview
Analysis of student academic performance data to understand how demographic factors and parental background influence student scores in Math, Reading, and Writing. Statistical visualizations like heatmaps and boxplots are used to uncover patterns.

 Objective

Analyze gender distribution across students
Study how parent's education level impacts student scores
Examine the effect of parent's marital status on academic performance
Detect outliers in Math, Reading, and Writing scores
Understand the distribution of students across ethnic groups


 Dataset
DetailInfoFileStudent_Score.csvKey ColumnsGender, ParentEduc, ParentMaritalStatus, MathScore, ReadingScore, WritingScore, EthnicGroup, WklyStudyHours

 Tools & Libraries
ToolPurposePythonCore programmingPandasData loading, cleaning, groupingNumPyNumerical computationsMatplotlibBase plottingSeabornHeatmaps, boxplots, count plots

 Data Cleaning Steps

Dropped unnamed index column (Unnamed: 0)
Fixed data entry error in WklyStudyHours column: "05-Oct" → "5-10"
Checked for null values using isnull().sum()


 Visualizations
ChartDescriptionCount PlotGender distribution of studentsHeatmapParent's education level vs average Math, Reading, Writing scoresHeatmapParent's marital status vs average scoresBoxplotScore distribution and outliers for MathBoxplotScore distribution and outliers for ReadingBoxplotScore distribution and outliers for WritingPie ChartDistribution of students across ethnic groups (A to E)Count PlotEthnic group count comparison

 Key Insights

Students whose parents have higher education (Master's/Bachelor's) score significantly better
Parent's marital status shows a slight variation in student performance
Math scores have a wider spread with more outliers compared to Reading and Writing
Group C and D are the most represented ethnic groups in the dataset
Female students tend to perform better in Reading and Writing, while scores are competitive in Math


 Project Structure
student-performance-analysis/
│
├── Student_score.ipynb     # Main analysis notebook
├── Student_Score.csv       # Dataset
├── README.md               # Project documentation

 How to Run

Clone this repository
Install required libraries:

bash   pip install pandas numpy matplotlib seaborn

Open Student_score.ipynb in Jupyter Notebook or VS Code
Run all cells
