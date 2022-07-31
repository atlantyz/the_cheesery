# The Cheesery

**Topic**: Texas Cheese Finder

**Dashboard**: [The Dashboard](https://www.google.com)

**Presentation**: [The Final Presentation](https://docs.google.com/presentation/d/1SVYNtrikItm9xgU9gQEdv__-XDalqVad2gs2nYSHae4/edit?usp=sharing)

## The Purpose


The purpose of this project is to create a database of Texas cheesemakers' cheese products, in addition to categorical cheese data, to find customers a Texas cheese they will enjoy. This project consists of the following elements: 

1. **The Database**: Create a database of cheese and cheesemakers from Texas. 
2. **The Dashboard**: Create an interactive dashboard that summarizes the cheese made and sold by Texas cheesemakers
3. **The Texas Cheese Finder**: The Texas Cheese Finder will use a supervised machine learning model to find a Texas cheese for customers based on cheese preferences for our new online cheese shop, The Cheesery.


## The Data and Database

### The Data

The data used to create the Texas cheese database was compiled from the Texas cheesemakers' websites and an online cheese database, containing categorical data that our team used to classify the Texas cheese. 

<img align = "right" img width="600" alt="Screen Shot 2022-07-27 at 2 30 16 PM" src="https://user-images.githubusercontent.com/79942792/181356334-cc9aeefa-6605-44a0-82ec-bd5dd8574ec8.png"
style="display: inline-block">

| **The List of Texas Cheesemakers**|
|-----|
| [The Mozarella Company](https://www.mozzco.com/) |
| [Veldhuizen Cheese](https://www.veldhuizencheese.com/)|
| [Cadence Creamery](https://www.cadencecreamery.com/)|
| [Rebel Austin](https://www.rebelcheese.com/)|
| [Haute Goat Creamery](https://www.hautegoatcreamery.com/)| 
| [Brazos Valley Cheese](https://www.brazosvalleycheese.com/) | 


**The Cheese.com Database**:

[Cheese.com](https://cheese.com/) 

### The Database

**The Entity Relationship Diagram**

Once our team created the Texas Cheese database, we created the Entity Relationship Diagram (ERD). The ERD denotes the data types of each category in our database--- 

<img
  src="https://user-images.githubusercontent.com/79942792/180083939-b64c0209-a2c6-4e79-b516-7f75ffcfce59.png"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
  

words words words 


<img width="500" alt="Screenshot 2022-07-20 120907" src="https://user-images.githubusercontent.com/79942792/180042079-ea880036-3d5a-490d-b32e-59b02a2bce42.png"> <img width="500" alt="" src="https://user-images.githubusercontent.com/79942792/181433420-fa44c26f-b6e8-447e-92f6-5595b0b77cfc.png">


## The Machine Learning Model

**Model Used**: KNNeighborClassifier

The purpose of this study is to find a Texas Cheese for customers. Our team used supervised machine learning *** more words.

| Preliminary feature selection and engineering | Preliminary data preprocessing |
| ------ | ----- | 
| Review colmuns for nulls and data types | Reviewing value_counts of data; This helped to determine potental target data within the dataset |
| Adjust column names to fit in with database | Realized that using 'cheese name' would create issues when trying to encode variables and run model |
| Drop null values (needed for clean data) | Encoded data using OneHotEncoder, fit and transformed the data |
| Checked unique values for each feature to determine which would be best for use | Adjusted the working dataset to contain only fields used by machine learning model |
| | Split preprocessed data into our feature and target arrays |


### Training the Model
- Split the preprocessed data into a training and testing dataset for the ML model
- Fit the data and run beginning predictions


## The Dashboard
Using Tableau and the dashboard, customers are able to:
* Filter elements of the dashboard and see how others are affected.
* Learn more about cheese and its characteristics


![tableau](https://github.com/rryl/the_cheesery/blob/aa865e2a0469306d7b50e47f352215a821f006d6/resources/CheeseryTableau.png)

Elements:
* Location Distribution
* Vegetarian Percentage
* Flavor Count
* Avg Price by Milk
* Avg Price by Family
* Interactive Map of the Cheese Companies

![ezgif com-gif-maker](https://user-images.githubusercontent.com/79942792/181353232-8674abc2-c5ea-4526-92b0-58a8100db0d8.gif)

## The Results

words words words

## The Conclusion

words words words

---
### The Project Details

**The Communication Protocol**

<img width="421" alt="Screenshot 2022-07-20 120612" src="https://user-images.githubusercontent.com/79942792/180041510-3b7aa78c-9654-4288-834e-636596b5b1b2.png">
