# The Cheesery

**Topic**: Texas Cheese Finder

**Dashboard**: [The Dashboard](https://public.tableau.com/views/TheCheesery_16589442131650/TheCheesery?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

**Presentation**: [The Final Presentation](https://docs.google.com/presentation/d/1SVYNtrikItm9xgU9gQEdv__-XDalqVad2gs2nYSHae4/edit?usp=sharing)

## The Purpose


The purpose of this project is to create a database of Texas cheesemakers' cheese products, in addition to categorical cheese data, to find customers a Texas cheese they will enjoy. This project consists of the following elements: 

1. **The Database**: Create a database of cheese and cheesemakers from Texas. 
2. **The Dashboard**: Create an interactive dashboard that summarizes the cheese made and sold by Texas cheesemakers
3. **The Texas Cheese Finder**: The Texas Cheese Finder will use a supervised machine learning model to find a Texas cheese for customers based on cheese preferences for our new online cheese shop, The Cheesery. Without the ability to taste the flavors offered online, this allows customers to get a list of cheeses similar to their already prefence and keep them shopping locally in Texas.

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
<img align = "right" width="200"
  src="https://user-images.githubusercontent.com/79942792/180083939-b64c0209-a2c6-4e79-b516-7f75ffcfce59.png"
  style="display: inline-block">

Once our team created the Texas Cheese database, we created the Entity Relationship Diagram (ERD). The ERD denotes the data types of each category in 
our database to conceptualize the columns that we are using in a different way. 



Through using the Entity Relationship Diagram that is shown we are able to view the completed process of going through all three of the ERD types: 
* the Conceptual diagram
* the Logical diagram
* the Physical diagram
  



The database was created using PostgreSQL and pgAdmin. In the database, we have various categories that consist of the names of the different 
cheeses, the different Texas cheese companies, the location of where the cheeses can be found in Texas, the typical prices of the cheeses, the different
kinds of milk that are used to make the different cheeses, the origin is where the cheeses are known to originate from. Some of the other columns are 
split up by cheeses can be categorized by the family of the cheese, the types of cheese, the different textures of cheese, along with the different 
colors, flavors, and the last column that we have available would be to tell if there is a vegetarian option for said cheese.


<img width="500" alt="Screenshot 2022-07-20 120907" src="https://user-images.githubusercontent.com/79942792/180042079-ea880036-3d5a-490d-b32e-59b02a2bce42.png"> <img width="500" alt="" src="https://user-images.githubusercontent.com/79942792/181433420-fa44c26f-b6e8-447e-92f6-5595b0b77cfc.png">


## The Machine Learning Model

**Model Used**: KNNeighborClassifier

The purpose of this study is to find a Texas Cheese for customers. Our team used supervised machine learning *** more words.


**Pros and Cons of Choosing KNN**
| Pros | Cons |
| ---- | ---- |
| Great for classification models with many different labels | The algorithm is a lazy learner and is prone to overfitting |
| Versatile in calculations of proximity | Computationally inefficient |
| More intuitive algorithm compared to other classification models | Difficult to find the 'right' value for "k" |
| Memory-based approach | |


<img width="500" src="https://user-images.githubusercontent.com/79942792/182504548-81ec29a0-a442-4366-a214-8e6bb10886b6.jpg"><img width="500" src="https://user-images.githubusercontent.com/79942792/182504733-c6978d73-6e53-47b3-a435-41f50a8a99a4.jpg">


**Training the Model**
- We defined the target as 'origin' or Cheese family and the features as the rest of the columns in our model. The other columns consist of characteristics that would help predict the correct Cheese family based on descriptions of each Cheese from our Texas-based companys.
- Split the preprocessed data into a training and testing dataset for the ML model. We chose to split it 80% training and 20% testing. 
- We created the StandardScaler instance, fit the scaler with the training set, and scaled the data for our model.
- Before we started to fit the model, we set up arrays to store the training and testing accuracies. Then, we plotted the accuracy scores with given parameters for the model to see at which point n_neighbors would equal a specfic parameter to give us our best accuracy. This number ended up as 1.
- Next, we fit the data and began running predictions.
- After making predictions on the testing data, we analyzed how well our knn model classifies Cheese family ('origin') by creating a Classification report that gives measures of: Accuracy, Precision, Recall, and F1-Scores.


## The Results

- As of now, our accuracy stands at 75%. While this is normally a good accuracy score, as you can see below some of our families have a 0 or 1. This is not good because it means our model had some overfitting or not enough data at all to make predictions needed.
- While our model could be a decent predictor of Cheddar or Mozzarella, it is not for any of the other families. This is likely due to under representation of the families in our dataset.

![Results of ML D3](https://user-images.githubusercontent.com/97268254/182053723-a93370a8-b1a2-42f5-9a0e-9a67780b683f.PNG)


## The Conclusion



## The Dashboard

<img width="800" alt="Screen Shot 2022-08-02 at 2 03 10 PM" src="https://user-images.githubusercontent.com/79942792/182455329-9331de6e-cd91-4a80-8a37-57feceb1270b.png">


<img width = "500" src="https://user-images.githubusercontent.com/79942792/182457580-015d684d-805e-404b-8eb3-902214e78f41.gif"> <img width = "500" src="https://user-images.githubusercontent.com/79942792/182457590-22d59079-7a3e-4821-9a37-4e9aafaed93e.gif">


<img width="500" alt="Screen Shot 2022-08-02 at 2 02 58 PM" src="https://user-images.githubusercontent.com/79942792/182455352-8f97f124-b071-414d-9f38-1b2d8cc8218d.png"> <img width="500" alt="Screen Shot 2022-08-02 at 2 03 04 PM" src="https://user-images.githubusercontent.com/79942792/182455360-afe319bd-b700-4866-9f25-8112d7f080a4.png">

---
### The Project Details

**The Communication Protocol**

<img width="421" alt="Screenshot 2022-07-20 120612" src="https://user-images.githubusercontent.com/79942792/180041510-3b7aa78c-9654-4288-834e-636596b5b1b2.png">
