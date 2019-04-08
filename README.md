# myrepo91
Data Analysis

Imported the dataset information.

Check to find out the number of rows and columns using df.shape

Find out the detailed description for all the available columns by df.describe

df.dtypes to check if there are any incorrect categories 

df.nunique() to check the number of unique values

df.info() to find out the information of the dataset including the number of rows and columns, raneg index, data types and memory usage

df.isnull().sum() to find out the sum of null values in all the columns

in [14] shows dropping the not useful columns and handling missing data

DATA CLEANING

check if there are any duplicates df.duplicated().sum()

Visualizing each variable to get statistics to each column to get a diagrametic representation using box plots

in[19] plotting the relation between budget and popularity and visualize it with scatter plot

based on median budget value to divide the budget into two groups : low and high
m = df['budget'].median()
low_budg =  df.query('budget < {}'.format(m))
high_budg =  df.query('budget >= {}'.format(m))

EXPLORATORY DATA ANALYSIS

checking the mean popularity of low and high budgets

with the attained values we create a bar chart

Created 3 groups with query().  <60 min: short   , 60 min <=  <= - 120 min: medium ,  >120 min: long
