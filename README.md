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

What_AI_Used_For.md:
Describes in detail how I used AI to help with issues with the project.

## Business Requirements

- Describe your business requirements

## Hypothesis and how to validate?

- Sales differences between holiday and non-holiday weeks per store
  Validation: Compare sales using statistical analysis and visualisation techniques.
- What is most profitable store type?
  Validation: Calculate monthly sales and compare across store types.
- Does temperature affect monthly sales?
  Validation: Use correlation analysis to determine the relationship between temperature and sales.
- Impact of markdowns on sales during holidays versus non-holiday periods
  Validation: Compare markdown data before and after the different periods.
- Compare sales performance across different stores
  Validation: Analyze sales across stores types.

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

## Unfixed Bugs

- Please list any unfixed bugs and explain why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
- Did you recognise gaps in your knowledge, and how did you address them?
- If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap

### Challenges and Strategies

- installing dependencies from requirements.txt file produced error:  
  ModuleNotFoundError: No module named 'pkg_resources'  
  So had to install dependencies manually using pip install <package_name>.
  THEN after checking with course fascilitator needed to remove ppscore from the requirements.txt file
  This produced another error which I tracked down to being ydata-profiling so removed that as well
  Re-installed dependancies from the requirements.txt file - works fine.
- VS Code repeatedly has a kernel hang randomly during development requiring restarting VS Code  
  as kernel restart rarely fixed the issue.

- What challenges did you face, and what strategies were used to overcome these challenges?
- What new skills or tools do you plan to learn next based on your project experience?

## Main Data Analysis Libraries

- os
- numpy
- pandas
- plotly.express
- seaborn
- matplotlib.pyplot

## Credits

- In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials; however, it is important to be very specific about these sources to avoid plagiarism.
- You can break the credits section into Content and Media, depending on what you include in your project.

### Content

- The text for the Home page was taken from the Wikipedia Article A
- Instructions on how to implement form validation were taken from a [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site

## Acknowledgements (optional)

- Thank the people who supported this project.
