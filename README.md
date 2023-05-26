# Grid_Search_CV
# First i import and load my iris data into columns, it will be my dataframe "pd.DataFrame(iris.data, columns = iris.feature_names)"
# Flower name will be my target columns, so I create this columns "df['flower'] = iris.target"and apply flower names to my column
# "df['flower'].apply(lambda x : iris.target_names[x])", then I check if it work by looking at my data with two different flower names 
