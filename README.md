# Grid_Search_CV
# First i import and load my iris data into columns, it will be my dataframe "pd.DataFrame(iris.data, columns = iris.feature_names)"
# Flower name will be my target columns, so I create this columns "df['flower'] = iris.target"and apply flower names to my column
# "df['flower'].apply(lambda x : iris.target_names[x])", then I check if it work by looking at my data with two different flower names 
# Now when I have my dataframe and target column I can import "train_test_split" and get "train and test set" of my data, X as "iris.data" y as "iris.target"
# Then before i use "Grid Search CV" I gonna write my code without it, so I import "SVC" model "kernel as rbf" "C will be 30" and "gamma = auto"
# This parameters are just a try, then I train my model "model.fit(X_train, y_train)" and check score "model.score(X_test, y_test)"
# I gonna check different parameters with "cross_val_score", so I supply into my "cross_val_score" same model with different parameters
# "cv" its the number of iterations, I get some different five scores "cv=5" from my "cross_val_score"
# Now I import "GridSearchCV" and put into my classifier "SVC" model, I set parameter "gamma to auto" and now I can check different parameters of my model 
# I set parameter "C at thre numbers [1, 10, 20]", then parameter "kernel to ['rbf','linear']" and "cv at 5, so it gonna take 5 different trys"
# "return_train_score = False" means that it will not include training scores, then I train my classifier with "X and y" as (iris.data, iris.target)
