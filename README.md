# JOB-A-THON

The solving the project in a simple way to approch the required solution,
following steps are applied.
  1. read the problem statement and data
  2. import the required libraries
  3. data cleaning
  4. EDA
  5. module approch
  6. comparision of trained and test data
  7. creating the sumbmission file

__Reading the problem statement__
the problem statement is to predict the Sales prize based on store types, location types, holidays and discounts

__Importing the data__
Asusale the data reading libraries are imported like pandas,
and some maths libraries like numpy, maths
for scaling the purpose the MinMax scalar,
and at last machine learning libraries from sklearn

__Data cleaning__
the data is checked weather the null values are present are not. but in this WOmart data set their is no null values present.
and check the independent and dependent columns.

__EDA__
the 1st approch in this step is to visualize the all the columns with each other, how they are corelated with each other.
the date column is an object data type so we do it in either int or float by spliting it in three other columns like day,month, year.
after this we do label encoder to all objective/categorical data type columns.
then we split the data in two data frames one in independent and another one in dependent.
in independent columns the ID and #Order column is removed beacuse one have all uniques vales with objective data type and its not effect the remaining module, and another one for matching the test and train data shape,(either remove it or compress the data features)
the independent column is scaled with the help of Minmax theorm.
then split it into training and testing data

__Module approch__
to check which module performs well for this data we imported 6 machine learning modules like RandomForest, XGB Regressor, Lasso and Ridge etc.
created a for loop were to check the all modules and listed out in  RMS values
comparing all the RMS vlaue the XGB Regressor gives less errors.

__comparision of trained and test data__
comparing the splited X_train and Y_train with visualization and r2 score

__creating the sumbmission file__
comparing all the RMS vlaue the XGB Regressor gives less error. so created a separate module to predict the test data set and created submissinon file with column names of ID and Sales, saved into '.csv' file.




**Thank you**
