# The Cheesery


Overview
----
### Description

For this project, we created a database of cheeses made and sold in Texas, from a variety of Texas cheesemakers. Our new online shop, The Cheesery, will use this database to create a machine learning model that will be able to identify Texas-based cheeses based on price and flavor. This project will provide engaging visualizations and a fun recommendation survey.

### Background

The Cheesery is an online cheese shop that highlights cheeses from Texan cheesemakers. Because these cheeses are primarily available in Texas, new customers may not be familiar with the flavor and texture of these cheeses. Thus, we created an extensive database of Texas-made cheeses to help new customers choose a Texas cheese for them based on general cheese characteristics. 

Framework
----
### Communication Protocol

<img width="421" alt="Screenshot 2022-07-20 120612" src="https://user-images.githubusercontent.com/79942792/180041510-3b7aa78c-9654-4288-834e-636596b5b1b2.png">

### Source Data

Following extensive research, we created a database that detailed the variety of cheeses that are made and sold in Texas, by Texan cheesemakers. In addition to the details of individual cheeses from the Texas cheesemakers, we added general cheese data, including cheese family and texture, from Cheese.com. 

This data contains specific and general details of cheese from Texan cheesemakers:
* Location: Where in Texas the cheesemaker is located. 
* Company: The Texas cheesemaker's business name.
* Cheese identification details: price, milk type, cheese family, (traditional) country of origin, type, texture, etc.

<img width="674" alt="Screenshot 2022-07-20 120907" src="https://user-images.githubusercontent.com/79942792/180042079-ea880036-3d5a-490d-b32e-59b02a2bce42.png">


### Data Focus

#### Flavor

The most important aspect of a food product is the taste! The goal of this project is to be able to accurately suggest a Texas cheese that new customers will enjoy based on similar cheese flavor and texture. 

#### Price

The price of each cheese can be a determining factor for new customers. Thus, our Texas Cheese database includes cheeses with a range of prices (by ounce) so that all customers can find a Texas cheese for their budget. 

#### Location

The Cheesery is an online cheese shop focused on cheese created in Texas.  

Machine Learning Model
----

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

### About our model
- Model Used: KNNeighborClassifier

Advantages:
- Successful in handling classification data that is not binary
- Known for being useful in large datasets

Limitations:
- Has trouble reading some data types
- Takes a large amount of computing power





Database
----

### Description of database

Database chosen: SQL via PGadmin

![QuickDBD-export (2)](https://user-images.githubusercontent.com/79942792/180083939-b64c0209-a2c6-4e79-b516-7f75ffcfce59.png)

![The_Cheesery's_Database](https://user-images.githubusercontent.com/79942792/180083945-3652d26e-ed0c-423d-8c0d-8f54115062a9.png)

The Texas Cheese database was created by our team to include Texan cheesemakers, location, cheeses sold, price, cheese family, flavor, and more.

Analytic Process
----

### Data Exploration Phase

Data was compiled using the information avaialble on Texas cheesemker's websites and the Cheese.com reference cheese catalog. 

Data from Texas Cheesemakers includes:
* Company name
* Location
* Cheese name
* Price
* Cheese description
* Milk type
* Cheese color

Data from Cheese.com includes: 
* Traditional country of origin
* Cheese family
* Cheese type

### Data Analysis Phase
### Tools Used

Presentation
----

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


## Google Slides



Results
----

Conclusion
----

## Recommendations

## Links
Tableau Dashboard: https://public.tableau.com/app/profile/alisha.lopez/viz/CheeseryAnalysis/Dashboard1?publish=yes
Google Slides: https://docs.google.com/presentation/d/1Q1fYu6wri5ixYhDtw178P070nDuyyvgeQGAQY8FjWeA/edit#slide=id.p
