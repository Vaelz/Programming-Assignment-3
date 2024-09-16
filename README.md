# Programming-Assignment-3

## Problem 1
#### Function/s Used:
  - import pandas as pd
  - pd.read_csv()
  - pd.head()
  - pd.tail()
  - %store

#### Documentation:
a. Importing Pandas as pd
  - Initially import the pandas library using import pandas as pd to access pandas functions.

b. Extracting cars CSV file
  - Extract the cars.csv file from the folder using pd.read_csv('cars.csv').

c. Display the first 5 data in the data frame
  - Using cars.head() function will display the first 5 (rows 0-4) data from the data frame.

d. Display the last 5 data in the data frame
  - Using cars.tail() function will display the last 5 (rows 0-4) data from the data frame.

Note: 
  - I used the %store function to store the variable in the database in which to use it for the other file.
  - I researched that %store only works in jupyter notebook and Ipython.
  -  This is also why i cant save the file as .py

## Problem 1
#### Function/s Used:
  - import pandas as pd
  - pd.loc [([])]
  - %store -r

#### Documentation:
a. Importing Pandas as pd
  - Initially import the pandas Library using import pandas as pd to access pandas functions.

b. Extracting the data frame cars
  - Extract the data frame cars from Problem 1 using %store -r cars (read note below) from the database.

c. Display the first 5 rows with odd number columns in the data frame
  - Using cars.loc[0:4,['mpg','disp','drat','qsec','am','carb']] function will display the first 5 rows of the selected columns (which right here is the odd columns) from the data frame.

d. Display the row of the Model Mazda RX4
  - Using cars.loc[0] function will display the car model Mazda RX4 row in a series format.
  - On the other hand, using the function cars.loc[cars['Model']=='Mazda RX4'] will also display the row of the car model, but it is in data frame format.

e. Looking for how many cylinders of a specific model (here is the model Camaro Z28)
  - Using cars.loc[(cars['Model']=='Camaro Z28'),['cyl']] function will look for the model that has 'Camaro Z28' in the dataset, then display its cylinder using 'cyl'.

f. Looking for the specific categories of a specific model/s of cars.
  - For the model Mazda RX4 Wag, using cars.loc[(cars['Model']=='Mazda RX4 Wag'),['Model','cyl','gear']] function will display the 'model', 'cylinder' and 'gear' for Mazda RX4 Wag.
  - For the model Ford Pantera L, using cars.loc[(cars['Model']=='Ford Pantera L'),['Model','cyl','gear']] function will display the 'model', 'cylinder' and 'gear' for Ford Pantera L.
  - For the model Honda Civic, using cars.loc[(cars['Model']=='Honda Civic'),['Model','cyl','gear']] function will display the 'model', 'cylinder' and 'gear' for Honda Civic.

Note:
- According to what I learned, the pd.loc[] function can be used in many ways in which to generally cut and/or remove the data frame
- Previously, the %store function was used to store the variable 'cars' in the database. Using %store -r cars, the variable 'cars' will be extracted from the database.
- Again, this only works for jupyter notebook and Ipython.

## Updates:
- Initial Post
- Added ReadMe File
- Added cars.csv File
- 
