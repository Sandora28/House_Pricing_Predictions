# House_Pricing_Predictions

Task - Predict the prices of houses in california based on given data.


in repository we can see already performed task in jupyter notebook (stuff that i have made in it is decribed down below).
and there is also second file , house.csv where u can see all the data which i have used to perform predictions.


describing performed commands and ideas - first of all , we should start with reading the data and analyze it with first look. based on data creating new train data
where we should perform all the stuff to reach the goal and get best score of model.
as we've seen on train data histograms there are too much skewed grahs so i used logarithms in order to balance the values of
some neccesary columns.
then i've analyzed correlation graph which shows that median income is mostly dependent thing to evaluate  house values
also there is ocean proximity column which where the house is allocated - near the beach , inland or something like that.  Of
course i noticed that ocean proximity would be best term for measuring house prices, so used get_dummies for recreaing boolean or just 1-0s for values of this column , in order to use it in model.
then as scatterplot and as correlation graph shows house near the ocean , or on the beach are much more expensive then inland houses - so it will have key performance on our model.
lastly, i create two model one with linear regression and second with randomforestregressor , that give us now to bad but not also best score for predicting the house values.
