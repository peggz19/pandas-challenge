# pandas-challenge

Hello and welcome to Peggy Tadi's pandas challenge.

When creating the School Summary Table, I didn't find how to merge series into Data Frames hence the long calculations to turn the groupby series into singular DataFrames before merging them all into a big one.
Later on, when doing the Math Score by Grade, I was able to find who to merge series into a DataFrame.

See below the links of the formulas I used but we didn't learn in class :

nunique () - https://www.statology.org/pandas-count-unique-values/#:~:text=You%20can%20use%20the%20nunique,values%20in%20a%20pandas%20DataFrame.

first() - https://stackoverflow.com/questions/68091878/pandas-get-unique-values-in-one-column-based-off-of-another-column-python

per_school_summary = reduce(lambda a,b: pd.merge(a,b, on = 'school_name', how='outer'),per_school_list) - https://stackoverflow.com/questions/52223045/merge-multiple-dataframes-based-on-a-common-column 

pd.concat() - https://sparkbyexamples.com/pandas/pandas-create-dataframe-from-multiple-series/