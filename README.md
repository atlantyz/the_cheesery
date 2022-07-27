# The Cheesery

**Topic**: Texas Cheese Finder

**Dashboard**: [The Dashboard](https://www.google.com)

**Presentation**: [The Final Presentation](https://www.google.com)

## The Purpose


The purpose of this project is to create a database of cheese, made and sold in Texas, to create an interactive dashboard and to use machine learning to find a Texas cheese for customers based on cheese preferences for our new online cheese shop, The Cheesery.


## The Data and Database

### The Data

words words words

**The List of Texas Cheesemakers**:

[The Mozarella Company](https://www.mozzco.com/)

[Veldhuizen Cheese](https://www.veldhuizencheese.com/)

[Cadence Creamery](https://www.cadencecreamery.com/)

[Rebel Austin](https://www.rebelcheese.com/)

[Haute Goat Creamery](https://www.hautegoatcreamery.com/)

[Brazos Valley Cheese](https://www.brazosvalleycheese.com/)

**The Cheese.com Database**:

[Cheese.com](https://cheese.com/)

### The Database

words words words
<img
  src="https://user-images.githubusercontent.com/79942792/180083939-b64c0209-a2c6-4e79-b516-7f75ffcfce59.png"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
  


<img width="400" alt="Screenshot 2022-07-20 120907" src="https://user-images.githubusercontent.com/79942792/180042079-ea880036-3d5a-490d-b32e-59b02a2bce42.png"> <img width="400" alt="" src="https://user-images.githubusercontent.com/79942792/180083945-3652d26e-ed0c-423d-8c0d-8f54115062a9.png">


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

## The Results


## The Conclusion


---
### The Project Details

#### The Communication Protocol

<img width="421" alt="Screenshot 2022-07-20 120612" src="https://user-images.githubusercontent.com/79942792/180041510-3b7aa78c-9654-4288-834e-636596b5b1b2.png">
