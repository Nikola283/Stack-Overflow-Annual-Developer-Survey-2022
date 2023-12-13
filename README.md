![survey_image](https://github.com/Nikola283/Stack-Overflow-Annual-Developer-Survey-2022/assets/76962010/77564f27-3eda-4fc9-885b-ad0ef8fb167b)
Stack Overflow Developer Survey Analysis
This repository contains Python code for analyzing the Stack Overflow Developer Survey 2022 dataset. The analysis focuses on various aspects of developers' preferences, experiences, and demographics.

Prerequisites
Python (3.7 or higher)
Jupyter Notebook (optional, but recommended)
Libraries Used
 pandas
 matplotlib
 plotly.express
 kaggle
Dataset Download
To run the code, you need to download the Stack Overflow Developer Survey 2022 dataset using the Kaggle API. Use the following command:

bash
Copy code
!kaggle datasets download -d dheemanthbhat/stack-overflow-annual-developer-survey-2022
Dataset Extraction
After downloading the dataset, unzip it using the provided Python code:

python
Copy code
import zipfile

zipfile_name = 'stack-overflow-annual-developer-survey-2022.zip'
with zipfile.ZipFile(zipfile_name, 'r') as file:
    file.extractall()
Data Analysis
The analysis includes several visualizations and insights. Here are some examples:

Remote Working Preferences

How much does remote working matter to employees?
python
Copy code
df['RemoteWork'].value_counts()
plot_df(df, 'RemoteWork', 'black')
Coding Experience vs. Compensation

How does coding experience affect the level of pay?
python
Copy code
# Code to calculate and visualize coding experience vs. compensation
Learning to Code

What's the most popular method of learning to code?
python
Copy code
df['LearnCode'].value_counts()
plot_df2(df, 'LearnCode', 'green')
Education Level and Job Opportunities

Are you more likely to get a job as a developer if you have a master's degree?
python
Copy code
df['EdLevel'].value_counts()
plot_df(df, 'EdLevel', 'blue')
Geographic Distribution

Geographic distribution of respondents
python
Copy code
df['Country'].value_counts()
plot_df(df, 'Country', 'blue')
Developer Types

Types of developers and their distribution
python
Copy code
df['DevType'].value_counts()
plot_df2(df, 'DevType', 'yellow')
Programming Languages

Programming languages developers have worked with
python
Copy code
df['LanguageHaveWorkedWith'].value_counts()
plot_df2(df, 'LanguageHaveWorkedWith', 'orange')
Gender Distribution

Gender distribution among respondents
python
Copy code
# Code for gender distribution pie chart
Company Size vs. Compensation

At what company size do developers get paid the most?
python
Copy code
# Code for company size vs. compensation analysis
License
This project is licensed under the MIT License - see the LICENSE file for details.

Feel free to explore and modify the code for your own analyses!
