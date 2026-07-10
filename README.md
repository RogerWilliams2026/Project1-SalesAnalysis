# Project 1 - Sales Analysis

**Project XYZ** is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Dataset Content

Dataset contains 3 related CSV files:

- Sales_Stores_DataSet.csv
- Sales_Features_DataSet.csv
- Sales_DataSet.csv

Project Folder Structure:

- Data <- No files stored here
- Data/CleanedDataSets <- Contains cleaned data as csv files
- Data/OriginalFiles <- Contains the original data csv files
- Data/VisualisationDataSet <- Contains a combined csv file for visualisation
- Documents <- Contains file: What_AI_Used_For.md (terrible grammar)
- Jupyter_Notebooks <- Contains the Jupyter Notebooks used for ETL and Visualisation

Jupyter_Notebooks:
There are separate notebooks for ETL on each csv file. THis was done so I can make sure each csv file is processed correctly which is easier to debug in one small notebook than a huge notebook with allthe csv files in.

Notebook Files:

- Notebook_ETL_Sales_Stores.ipynb <- ETL for Sales_Stores_DataSet.csv
- Notebook_ETL_Sales_Features.ipynb <- ETL for Sales_Features_DataSet.csv
- Notebook_ETL_Sales.ipynb <- ETL for Sales_DataSet.csv
- Notebook_ETL_Sales_Combined.ipynb <- Combines the 3 cleaned csv files into one for visualisation
- Notebook_Visualisations.ipynb <- Contains the visualisations for the hypotheses

What_AI_Used_For.md:

Describes in detail how I used AI to help with issues with the project.

## Business Requirements

- Business requires insights into the generic performance of the business in certain key areas:
  - Are sales increased if weather is hotter or colder?
  - What are the sales differences between holiday and non-holiday weeks per store?
  - What is most profitable store type?
  - Does store size affect profitability? If so, how much?
  - What affect does markdowns have on sales during holidays versus non-holiday periods?

The business hopes this basic information will help it plan its store growth and marketing strategies to maximise profits in the areas that are shown to be profitable, but also focus on improvement for the stores that are not performing well.

## Hypothesis and how to validate?

- Are sales increased if weather is hotter or colder in the last 12 months?
  Validation: Test with a suitable plot to show temperature and sales correlation.
- Sales differences between holiday and non-holiday weeks per store in the last 12 months
  Validation: Compare sales using statistical analysis and visualisation techniques.
- What is most profitable store type in the last 12 months?
  Validation: Compare store types with weekly sales.
- Does store size affect profitability? If so, how much in the last 12 months?
  Validation: Compare store size with weekly sales
-

- Impact of markdowns on sales during holidays versus non holiday periods in the last 12 months
  Validation: Compare markdown data before and after the different periods
-

Future Ideas:

- What are the most profitable departments per store?
- Some sort of report needing monthly values

## Project Plan

- Testing my knowledge of the KANBAN project management, is in with this GitHub project
- Outline the high-level steps taken for the analysis.
- How was the data managed throughout the collection, processing, analysis and interpretation steps?
- Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations

- List your business requirements and a rationale for mapping them to the Data Visualisations

## Analysis techniques used

From the 3 csv files 4 more are created 3 via ETL and 1 via merging the 3 cleaned csv files:

- Sales_Stores_DataSet_Cleaned.csv
- Sales_Features_DataSet_Cleaned.csv
- Sales_DataSet_Cleaned.csv
- Sales_Combined.csv

Methods Used:

-

- List the data analysis methods used and explain limitations or alternative approaches.
- How did you structure the data analysis techniques? Justify your response.
- Did the data limit you, and did you use an alternative approach to meet these challenges?
- How did you use generative AI tools to help with ideation, design thinking and code optimisation?

## Development Roadmap

### Basic Strategy:

- Start with basic plots to visualise the data then if have the time try ans expand and develop
  them further. Would be sweet to get some 3D plots in..

### Challenges and Strategies

- installing dependencies from requirements.txt file produced error:  
  ModuleNotFoundError: No module named 'pkg_resources'  
  So had to install dependencies manually using pip install <package_name>.
  THEN after checking with course fascilitator needed to remove ppscore from the requirements.txt file
  This produced another error which I tracked down to being ydata-profiling so removed that as well
  Re-installed dependancies from the requirements.txt file - works fine.
- VS Code repeatedly has a kernel hang randomly during development requiring restarting VS Code  
  as kernel restart rarely fixed the issue.
- First hypothesis raised an unexpected issue as some plot types would not render due to the data size!
  bar plots particularly fell at the first fence. Pity as that would have looked cool...
- trying to visualise plots with plotly.express produced an error stating nbformat was not installed.  
  Used pip install nbformat and added to dependencies in Notebook_Visualisations.ipynb to fix the issue

## New Skills and Tools

- Generative AI tools (Copilot and chatGPT) helped hugely with strange library issues and code snippets.
- Learned aboOt project management, and effective timeboxing for project sections e.g. documentation
- Discovered I preferred plotly as a visualisation tool due to its better appearence and options.

## Things To Learn Next

- Proper use of KANBAN for project management
- How to dynamically create ranges for subplots e.g. stores 1 to 9

- What challenges did you face, and what strategies were used to overcome these challenges?
- What new skills or tools do you plan to learn next based on your project experience?

## Main Data Analysis Libraries

- numpy
- pandas
- plotly.express
- seaborn
- matplotlib.pyplot

## Others Added By Me

- from matplotlib.ticker import MultipleLocator <- for "ticks" between axis values
- import nbformat <- added by me for plotly.express visualisation issue
- os <- for directory routines

## Unfixed Bugs

- Had strange issue with first plot in hypothessis 3, where it put: 1e9 in the top left corner of the
  plot. No idea why. Will have a look if there is a soultion if I have time does not affect plot data.
- Please list any unfixed bugs and explain why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
- Did you recognise gaps in your knowledge, and how did you address them?
- If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Credits

- Copilot quite useful for code snippets and ideas, but not always correct.
- chatGPT really good for solving code issues so far everything suggested worked!

## Acknowledgements (optional)

- Thank the people who supported this project.
