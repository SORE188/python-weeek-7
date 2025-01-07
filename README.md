

#  Basic Data Analysis

# Basic statistics for numerical columns
print("\nBasic statistics (mean, median, std, etc.):")
print(df.describe())

# grouping by a categorical column and computing the mean of a numerical column
# if 'species' is a categorical column and 'sepal_length' is a numerical column
if 'species' in df.columns and 'sepal_length' in df.columns:
    print("\nAverage sepal length for each species:")
    grouped_data = df.groupby('species')['sepal_length'].mean()
    print(grouped_data)
else:
    print("\nThe columns 'species' and 'sepal_length' do not exist in the dataset.")
    


