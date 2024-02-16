# datafun-06-eda
# Overview
 Project 6 is an opportunity to create your own custom exploratory data analysis (EDA) project using GitHub, Git, Jupyter, pandas, Seaborn and other popular data analytics tools.

 Created By Priyanka Naskar
 
 Date 2/12/2024
# Explore Datasets
ThisEDA will analyze the "penguins" dataset from the Seaborn library. It contains information about  diffrernt types pf penguin specis.you can found this data set in this belowe link

(https://github.com/mwaskom/seaborn-data/blob/master/penguins.csv)


# Deta set description
In this EDA  the penguins dataset  revealed valuable insights into the characteristics of different penguin species. First, let's load the dataset from the file "penguins.csv" using pandas and have a general overview of it.
Here is some table view of this data set

![alt text](image.png)

# Project Structure & Deliverables 

 README.md:  Provides an overview of the project and instructions for setting up the environment and running the notebook.

 requirements.txt: Lists all the Python packages required for the project.

 naskar_eda.ipynb  The Jupyter Notebook containing the EDA for the Planets dataset.

 # Environment Setup and How to Install and Run the Project

Create a new GitHub repository named datafun-06-eda.

Clone the repository to your local machine.

# git clone  (https://github.com/Priyankanaskar/datafun-06-eda)

# . Create a Project Virtual Environment in the .venv folder.

# . Activate the Project Virtual Environment.

# . Freeze your requirements to requirements.txt. 

py -m venv .venv
.\.venv\Scripts\Activate.ps1
py -m pip install requests
py -m pip freeze > requirements.txt


# .Install dependencies

py -m pip install jupyterlab numpy pandas matplotlib seaborn scipy pyarrow plotly bokeh scikit-learn holoviews datashader altair

 # Add a useful .gitignore to the root project folder.
 Start Jupyter: Do both methods. Both methods must be available.

 Method 1:
  Start Jupyter in VS Code: Open project folder in VS code, Install Jupyter extension in VS code (if not already installed), Open VS Code Terminal window, and run jupyter lab in integrated terminal.

 Method 2:
  Start Jupyter in Native Terminal (without VS Code): Open machine terminal in project folder, Start Jupyter Notebook server by running: jupyter lab; Default brower will open to Jupyter Notebook interface.

# Data Analysis Workflow
 The Jupyter Notebook follows a structured approach to EDA, consisting of the following steps:

# Data Acquisition: Loading the Planets dataset into a pandas DataFrame.

# Initial Data Inspection: Exploring the dataset's basic properties.

# Descriptive Statistics: Summarizing the central tendency, dispersion, and shape of the dataset's distribution.

# Data Distribution Analysis: Visualizing the distribution of data through histograms and count plots.

# Data Transformation and Feature Engineering: Enhancing the dataset with additional features and transformations for better analysis.

# Visual Analysis: Using various plots such as pairplots and heatmaps to visualize relationships between features.

# Storytelling and Presentation: Narrating the data story based on insights derived from the visual analysis.

# Conclusion: Summarizing the findings and the potential for further analysis.

# Contributing

 We welcome contributions to this project. If you have suggestions to improve the analysis or encounter issues, please open an issue or submit a pull request.

# References & Acknowledgments

Special thanks to OpenAI for assistance with project design and coding structure. Additional references used for this project include:

JUPYTER.md for Jupyter Notebook keyboard shortcuts and recommendations.

MARKDOWN.md for Markdown syntax and recommendations.

https://seaborn.pydata.org/tutorial.htmlfor visualization project ideas.

https://seaborn.pydata.org/tutorial.html for assistance with plotting functions.

And Special Thanks To Dr.Case https://github.com/denisecase/datafun-06-spec for complete guidence.