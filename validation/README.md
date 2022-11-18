
Read data from a csv and check the constraints. Sample data in data/train.csv and data/test.csv.

If constraints are met then return the data, if not raise an exception stating at least one failed row.

columns to read = ['Id','Street','YearBuilt','Fireplaces', 'FireplaceQu','1stFlrSF', '2ndFlrSF']

The checks:

 - id is int
 - Street column is a string
 - YearBuilt value is between 1700 and 1900.
 - firstfloor is at least one third of the 2nd floor
 - FireplaceQuality - FireplaceQu - optional - nullable - enum values of 'Ex', 'Gd', 'TA', 'Fa', 'Po'. If Fireplaces is greater than 0, FireplaceQu is required.
 

 Bonus:
 - id is unique



Try it with several frameworks - pandas, pydantic, Great Expectations, Pandera, mage, DBT.


## Credit

Exercises taken from a much more extensive tutorial and talk by Natan Mish
https://github.com/NatanMish/data_validation/

And inspired by a step in Laszlo's Titanic refactoring exercise  https://github.com/xLaszlo/CQ4DS-notebook-sklearn-refactoring-exercise


## Data

Datasetis taken from the [House prices 
prediction competition on Kaggle](https://www.kaggle.com/competitions/home-data-for-ml-course/data). 