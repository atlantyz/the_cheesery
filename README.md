# The Cheesery

**Topic**: Texas Cheese Finder

**Dashboard**: [The Dashboard](https://www.google.com)

**Presentation**: [The Final Presentation](https://www.google.com)

## The Purpose


The purpose of this project is to create a database of cheese, made and sold in Texas, to create an interactive dashboard and to use machine learning to find a Texas cheese for customers based on cheese preferences for our new online cheese shop, The Cheesery.


## The Data and Database

### The Data

Following extensive research, we created a database that detailed the variety of cheeses that are made and sold in Texas, by Texan cheesemakers. In addition to the details of individual cheeses from the Texas cheesemakers, we added general cheese data, including cheese family and texture, from Cheese.com. 

This data contains specific and general details of cheese from Texan cheesemakers:
* Location: Where in Texas the cheesemaker is located. 
* Company: The Texas cheesemaker's business name.
* Cheese identification details: price, milk type, cheese family, (traditional) country of origin, type, texture, etc.

<img width="674" alt="Screenshot 2022-07-20 120907" src="https://user-images.githubusercontent.com/79942792/180042079-ea880036-3d5a-490d-b32e-59b02a2bce42.png">

### The Database

![QuickDBD-export (2)](https://user-images.githubusercontent.com/79942792/180083939-b64c0209-a2c6-4e79-b516-7f75ffcfce59.png)


![The_Cheesery's_Database](https://user-images.githubusercontent.com/79942792/180083945-3652d26e-ed0c-423d-8c0d-8f54115062a9.png)

Cleaned Dataset
<img width="674" alt="Screenshot 2022-07-20 120907" src="https://user-images.githubusercontent.com/79942792/180042079-ea880036-3d5a-490d-b32e-59b02a2bce42.png">



![The_Cheesery's_Database](https://user-images.githubusercontent.com/79942792/180083945-3652d26e-ed0c-423d-8c0d-8f54115062a9.png)

## The Machine Learning Model

### About our model
**Model Used**: KNNeighborClassifier

Advantages:
- Successful in handling classification data that is not binary
- Known for being useful in large datasets

Limitations:
- Has trouble reading some data types
- Takes a large amount of computing power

### Preliminary feature selection and engineering
- Review colmuns for nulls and data types
- Adjust column names to fit in with database 
- Drop null values (needed for clean data)
- Checked unique values for each feature to determine which would be best for use 

### Preliminary data preprocessing
- Reviewing value_counts of data; This helped to determine potental target data within the dataset.
- Realized that using 'cheese name' would create issues when trying to encode variables and run model.
- Encoded data using OneHotEncoder, fit and transformed the data
- Then, adjusted the working dataset to contain only fields used by machine learning model
- Split preprocessed data into our feature and target arrays

### Training the Model
- Split the preprocessed data into a training and testing dataset for the ML model
- Fit the data and run beginning predictions


## The Dashboard
![dashboard](https://github.com/rryl/the_cheesery/blob/d139e25bc058936fcfbffe520e19cab4ce31d56e/resources/CheeseryTableau.png)

Using Tableau and the dashboard, customers are able to:
* Filter elements of the dashboard and see how others are affected.
* Learn more about cheese and its characteristics

Elements:
* Location Distribution
* Vegetarian Percentage
* Flavor Count
* Avg Price by Milk
* Avg Price by Family





## Results


## Conclusion


---
## Project Details

### Communication Protocol

<img width="421" alt="Screenshot 2022-07-20 120612" src="https://user-images.githubusercontent.com/79942792/180041510-3b7aa78c-9654-4288-834e-636596b5b1b2.png">
