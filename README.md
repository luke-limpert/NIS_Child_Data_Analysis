# NIS_Child_Data_Analysis
 NIS Child data analysis

Assignment 2 of the coursera "Data Science for Python".

The assignment makes use of an introduction to series, dataframes, regex, .where(), .loc, .iloc, pandas, numpy, boolean masking. 

Introduction to scipy in the final question of the assignment. 

Mostly used boolean masking, but another method was discussed in the lecture to overload the indexing operator.

df[df['HAD_CPOX']]

The .apply() method was also introduced where a function is used for every row in a column.

The example given reads:

def splitname(row):/n
	row['First']=row['President'].split(" ")[0]

df=df.apply(splitname, axis='columns')

Finally the .extract() method was also shown. 

After creating a regex pattern it will extract from a column and apply the pattern to each row. Afterwords a new column will be created for each capturing group. 

(?:) creates a non-capturing group. This excludes it. 

pattern = "(^[\w]+)" /n
df['President'].str.extract(pattern).head()

