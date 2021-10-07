# Pandas-Introduction
Pandas Introduction and It's various functions uses 
### Pandas

Pandas is a python library used for data manipulation , analyze , explore the data and get it ready for the machine learning .

Basically used for the data analysis part.

There are two types of datatypes that pandas have 

- Series
    - These are basically 1-Dimmensional . To create a series we need to give a list
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c1815768-a670-44cc-b141-4b933c8d10df/Untitled.png)
        
    - This is the resulting output of the series
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4d886660-272a-4035-8d91-f4f760e5aea6/Untitled.png)
    
- DataFrame
    - These are 2-dimmensional . These contains columns and are far more common than the series .
        
        For creating data frames we need to give the dictionary as input . We can also give series as the value as given below .
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/228d907a-5cb7-43bb-b61b-dc3a26081078/Untitled.png)
        
    - Resulting output for an dataframe
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1e3684d2-f7c1-4644-8998-8bfbcafae989/Untitled.png)
        
    

Importing data from csv

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/76a983c9-1958-4a2b-8a47-c95c61ed8196/Untitled.png)

This would result in the form of dataframes 

Exporting dataframe in the form of csv

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/80e4e0ee-aeab-4d53-9f5f-0bc3853c496f/Untitled.png)

If we don't give the index parameter it will create unnamed column of index by default so to avoid it we give index value as False 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/76f58417-643f-454e-bd7f-1ea5bd5fa437/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5b9c1b15-87b8-43ca-a53a-58be82567538/Untitled.png)

Important Commands in Pandas 

- car_dataset.head()
    
    This results in the top 5 rows in the output , we can change the number of rows by giving the number as an argument
    
- car_dataset.tail()
    
    This results in the last 5 rows in the output , we can change the number of rows by giving the number as an argument
    
- car_dataset.Info()
    
    This gives the information about the data types of the columns and number of columns in the dataframes 
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a0c6cd10-3118-4c2b-85d1-05359a13da29/Untitled.png)
    
- car_dataset.describe()
    
    This gives the statistical information about the dataframe for the columns whose datatypes is integers
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/41be751a-ee25-484f-afed-6f2c96f14ce1/Untitled.png)
    
- car_dataset.mean()
    
    This gives the mean for whole dataframe , if we want to get the mean for particular columns specify the name and then get its mean .
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b71d6db1-124d-4af9-a938-d24f5c801603/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f36059a4-f134-40be-a8cd-789df53b90ab/Untitled.png)
    
- car_dataset.sum()
    
    This results in the sum for the columns 
    
- pd.crosstab(car_dataset.Make , car_dataset.Doors)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e225de63-d709-42e1-8b87-5cae54541575/Untitled.png)
    
    This is used for comparing two columns and only is used for two columns not more than that
    
- car_dataset.loc[3]
    
    loc → refers to the index of the object in the dataframe or series 
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/54e519c6-b355-46e6-8187-4d9593b44582/Untitled.png)
    
- car_dataset.iloc[3]
    
    iloc → refers to the position of the object in the series or dataframe 
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/21d388e3-482e-407a-8c48-25fd4be21482/Untitled.png)
    
- car_dataset.groupby(car_dataset.Make)
    
    This is used for grouping the datframe by a particular column and then calculating results according to it.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9f018c19-63a0-4587-ab91-ef01222832cd/Untitled.png)
