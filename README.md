# datafun-06-eda
# Overview
 Project 6 is an opportunity to create your own custom exploratory data analysis (EDA) project using GitHub, Git, Jupyter, pandas, Seaborn and other popular data analytics tools.

 Created By Priyanka Naskar
 
 Date 2/12/2024

# Deliverable Names
GitHub Repository: datafun-06-eda

Documentation: README.md

Notebook: naskar_eda.ipynb

# Deta set description
This EDA will analyze The Iris Dataset is very simple often referred to as the Hello World. The dataset has 4 features of three different species of flowers namely Iris setosa, Iris virginica, and Iris versicolor. These features are sepal length, sepal width, petal length, and petal width. There are 150 data points in the dataset, 50 data points for each species.


# EDA on Iris Dataset
First, let's load the dataset from the CSV file "iris_csv.csv" using pandas and have a general overview of it.

The dataset can be downloaded from the below link.

https://www.kaggle.com/code/ash316/ml-from-scratch-with-iris


# External Dependencies
jupyterlab

pandas

pyarrow

matplotlib

seaborn

import matplotlib as plt
import pandas as pd
import seaborn as sns

# Exploratory Data Analysis
# Load the dataset into a pandas DataFrame - adjust this process for your custom data


df = pd.read_csv("iris_csv.csv") 
# Inspect first rows of the DataFrame

print(df.head())

The dataset contains information about iris flowers, including sepal length, sepal width, petal length, petal width, and species.Each row represents a unique iris flower, and the columns provide numerical measurements for different attributes.

# Initial Data Inspection

print(df.head(10))

print(df.shape)

print(df.dtypes)

This displays the first 10 rows of the DataFrame. It allows you to observe the initial records in the dataset, providing a snapshot of the data.

# Initial Descriptive Statistics

print(df.describe())

This function provides a summary of basic statistical measures for each numerical column in the DataFrame. 

# Initial Data Distribution for Numerical Columns

import matplotlib.pyplot as plt

import pandas as pd

import seaborn as sns


# Inspect histogram for a specific numerical column (e.g., 'sepal_length')

df['sepal_length'].hist()

# Inspect histograms for all numerical columns

df.hist()

# Show all plots

plt.show()

 This is Multiple histograms, one for each numerical column in the dataset.
A visual overview of the distributions of sepal length, sepal width, petal length, and petal width.
Insights into the central tendency, spread, and potential outliers in each numerical feature.

# Initial Data Distribution for Categorical Columns
# Inspect value counts by categorical column

df['species'].value_counts()

# Inspect value counts for all categorical columns

for col in df.select_dtypes(include=['object', 'category']).columns:
    # Display count plot
    sns.countplot(x=col, data=df)
    plt.title(f'Distribution of {col}')
    plt.show()

# Show all plots

plt.show()
This is histograme Shows the count of each unique species in the 'species' column.
Provides insights into the distribution of different iris species in the dataset.
# Rename one column

def rename_column(df, old_column, new_column):
    df = df.rename(columns={old_column: new_column})
    return df


# Rename the 'sepal_length' column to 'sepal_length_new'

df = rename_column(df, 'sepal_length', 'sepal_length_new')

print(df.dtypes)
Rename the column "sepal_length" to "sepal_length_new"

# Insert a new column 'new_column' with dummy values

df['beautification'] = 'yes'

# Print the DataFrame to verify the new column

print(df.head())

# Load the dataset into a pandas DataFrame - adjust this process for your custom data

df = sns.load_dataset('iris')

# Insert a new column 'new_column' with dummy values

df['colours'] = "red"

# Inspect first rows of the DataFrame

print(df.head())

Inthis colum I added one column "colours" with column value "red"
So, in this table sentosa colours red.

# Initial Visualizations

sns.pairplot(df, hue='species')
plt.show()

Observations: Pair Plot Analysis

The pair plot above provides a visual overview of the relationships between pairs of features in the Iris dataset, with different species distinguished by color.

Sepal Length and Sepal Width

Setosa species generally shows distinct clusters, especially in sepal length and sepal width. Versicolor and Virginica species exhibit some overlap, particularly in sepal length.

Petal Length and Petal Width

Clear separation between Setosa and the other species in petal length and petal width. Versicolor and Virginica show some overlap but are generally distinguishable.

Sepal Length vs. Petal Length

Positive correlation between sepal length and petal length across all species. Setosa generally has shorter petals compared to Versicolor and Virginica.

Sepal Width vs. Petal Width

No strong correlation between sepal width and petal width. Setosa has a smaller range in petal width compared to the other species.
General Insights

The pair plot highlights distinct patterns and relationships between features for different Iris species.

Petal measurements seem to be more effective in differentiating between species compared to sepal measurements.

These visualizations provide valuable insights that can guide further analysis and feature selection in the explorat


Push to github repository
In terminal comment git add . git commit -m"update README.md" git push origin main


# Contributing
We welcome contributions to this project. If you have suggestions to improve the analysis or encounter issues, please open an issue or submit a pull request.

# References & Acknowledgments
Special thanks to OpenAI for assistance with project design and coding structure. Additional references used for this project include

JUPYTER.md for Jupyter Notebook keyboard shortcuts and recommendations.

MARKDOWN.md for Markdown syntax and recommendations

Data Visualization using Python, Matplotlib and Seaborn for visualization project ideas.