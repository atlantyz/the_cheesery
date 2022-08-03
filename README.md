# The Cheesery

**Topic**: Texas Cheese

[The Dashboard and Interactive Map](https://public.tableau.com/views/TheCheesery_16589442131650/TheCheesery?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

[The Final Presentation](https://docs.google.com/presentation/d/1SVYNtrikItm9xgU9gQEdv__-XDalqVad2gs2nYSHae4/edit?usp=sharing)

## The Purpose


The purpose of this project is to create a database of Texas cheesemakers' cheese products, in addition to categorical cheese data, to find customers a Texas cheese they will enjoy. This project consists of the following elements: 

1. **The Database**: Create a database of cheese and cheesemakers from Texas. 
2. **The Texas Cheese Finder**: The Texas Cheese Finder will use a supervised machine learning model to find a Texas cheese for customers based on cheese preferences for our new online cheese shop, The Cheesery. Without the ability to taste the flavors offered online, this allows customers to get a list of cheeses similar to their already prefence and keep them shopping locally in Texas.
3. **The Dashboard**: Create an interactive dashboard that summarizes the cheese made and sold by Texas cheesemakers

## The Dataset and Database

### The Dataset

The data used to create the Texas cheese dataset was compiled from the Texas cheesemakers' websites and an online cheese database, containing categorical data that our team used to classify the Texas cheese. 

<img align = "right" img width="500" alt="Screen Shot 2022-07-27 at 2 30 16 PM" src="https://user-images.githubusercontent.com/79942792/181356334-cc9aeefa-6605-44a0-82ec-bd5dd8574ec8.png"
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

Once our team created the Texas Cheese database, we created the Entity Relationship Diagram (ERD). The ERD denotes the data types of each category in our database to conceptualize the columns that we are using in a different way. 


Through using the Entity Relationship Diagram that is shown we are able to view the completed process of going through all three of the ERD types: 
  * The Conceptual diagram - A visual representation of how the concept of a system works by using a title name for the table and column headers. This would be the first step in the ERD.
  * The Logical diagram - A graphical representation of a program that combines the conceptual diagram's information with all of the data types and the primary keys. This would be the second step that builds upon the Conceptual diagram
  * The Physical diagram - Explains how the conceptual and logical diagrams are connected through the data to appear as a physical correlation and this would be the last step of the ERD process 

  
**The Database**

The database was created using PostgreSQL and pgAdmin. In the database, we have various categories that consist of the names of the different 
cheeses, the different Texas cheese companies, the location of where the cheeses can be found in Texas, the typical prices of the cheeses, the different kinds of milk that are used to make the different cheeses, the origin is where the cheeses are known to originate from. Some of the other columns are split up by cheeses can be categorized by the family of the cheese, the types of cheese, the different textures of cheese, along with the different colors, flavors, and the last column that we have available would be to tell if there is a vegetarian option for said cheese.


<img width="500" alt="Screenshot 2022-07-20 120907" src="https://user-images.githubusercontent.com/79942792/180042079-ea880036-3d5a-490d-b32e-59b02a2bce42.png"> <img width="500" alt="" src="https://user-images.githubusercontent.com/79942792/181433420-fa44c26f-b6e8-447e-92f6-5595b0b77cfc.png">


## The Machine Learning Model

**Model Used**: K-Nearest Neighbor Classifier

To find customers of The Cheesery a Texas Cheese based on cheese classification data, we chose the supervised machine learning algorithm, the K-Nearest Neighbor Classifier (KNN). Because many of our customers will be new to the world of Texas Cheese, we used machine learning to find a cheese based on the characteristics of cheese they have tried before. The KNN algorithm assumes that similar things are in close proximity. Thus, we believed the KNN algorithm would be proficient in finding a Texas cheese that is similar to known cheese classifications. 


**Pros and Cons of Choosing K-Nearest Neighbor Classifier**
| Pros | Cons |
| ---- | ---- |
| Great for classification models with many different labels | The algorithm is a lazy learner and is prone to overfitting |
| Versatile in calculations of proximity | Computationally inefficient |
| More intuitive algorithm compared to other classification models | Difficult to find the 'right' value for "k" |
| Memory-based approach | Does not work well with large datasets|


<img width="500" src="https://user-images.githubusercontent.com/79942792/182509777-c3907349-0b52-42b1-9194-46a20c4c32f5.jpg"><img width="450" src="https://user-images.githubusercontent.com/79942792/182504733-c6978d73-6e53-47b3-a435-41f50a8a99a4.jpg">


**Training the Model**
- We defined the target as 'origin' or Cheese family and the features as the rest of the columns in our model. The other columns consist of characteristics that would help predict the correct Cheese family based on descriptions of each Cheese from our Texas-based companys.
- Split the preprocessed data into a training and testing dataset for the ML model. We chose to split it 80% training and 20% testing. 
- We created the StandardScaler instance, fit the scaler with the training set, and scaled the data for our model.
- Before we started to fit the model, we set up arrays to store the training and testing accuracies. Then, we plotted the accuracy scores with given parameters for the model to see at which point n_neighbors would equal a specfic parameter to give us our best accuracy. This number ended up as 1.
- Next, we fit the data and began running predictions.
- After making predictions on the testing data, we analyzed how well our knn model classifies Cheese family ('origin') by creating a Classification report that gives measures of: Accuracy, Precision, Recall, and F1-Scores.


## The Results

<img align = "right" width="300"
  src="https://user-images.githubusercontent.com/97268254/182053723-a93370a8-b1a2-42f5-9a0e-9a67780b683f.PNG"
  style="display: inline-block">
  
The K-Nearest Neighbor Classifier supervised machine learning model yielded an accuracy of 75%. The accuracy scores for cheddar cheese and mozzarella cheese families indicates that The Cheesery will be proficient in recommending a cheese that is similar to one of these cheese families. However, many of our cheese families have a score of 0 or 1. We determined that the scores of 0 or 1 are due to either overfitting or an insufficient amount of data in the dataset to make predictions for every cheese family.

**Recommendations**: 

We recommend that Texas cheesemakers make more cheese! While Texas is one of the top 5 cheese producing states, there is still a small amount of cheesemakers throughout Texas. As a result, we could not feed the model more information about cheeses that do not exist, yet! 


## The Dashboard

<img align = "right" width="500" alt="Screen Shot 2022-08-02 at 2 03 10 PM" src="https://user-images.githubusercontent.com/79942792/182455329-9331de6e-cd91-4a80-8a37-57feceb1270b.png" style="display: inline-block">

Our dashboard uses an interactive maps of Texas to illustrate the location of the Texas cheesemakers in our dataset. The interactive maps allow the user to select cheese characteristics such as cheese family, cheese price, and cheese flavor to find a Texas cheesemaker(s) that makes a cheese with the user-defined specifications. 

In addition to the interactive maps of Texas cheesemakers, our dashboard includes visualizations of our team's Texas Cheese dataset. The user can easily visualize information about Texas Cheese including: 

* Average Cheese Price by Cheesemaker
* Average Cheese Price by Cheese Family
* Average Cheese Price by Milk Type
* Number of Cheeses (in the Texas Cheese datset) by Cheese Family
* Number of Cheeses (in the Texas Cheese datset) by Milk Type
* Number of Cheeses (in the Texas Cheese datset) by Traditional Country of Origin
* Number of Cheeses (in the Texas Cheese datset) by Flavor



<img width = "500" src="https://user-images.githubusercontent.com/79942792/182457580-015d684d-805e-404b-8eb3-902214e78f41.gif"> <img width = "500" src="https://user-images.githubusercontent.com/79942792/182457590-22d59079-7a3e-4821-9a37-4e9aafaed93e.gif">


<img width="400" alt="Screen Shot 2022-08-02 at 2 02 58 PM" src="https://user-images.githubusercontent.com/79942792/182455352-8f97f124-b071-414d-9f38-1b2d8cc8218d.png"> <img width="400" alt="Screen Shot 2022-08-02 at 2 03 04 PM" src="https://user-images.githubusercontent.com/79942792/182455360-afe319bd-b700-4866-9f25-8112d7f080a4.png">


### The Conclusion

The online-concept store, The Cheesery, focused on cheese created throughout the state of Texas. Our team compiled data from Texas cheesemakers, and combined the available information with an existing dataset on Cheese.com. Following the creation of the Texas Cheese dataset, our team created a database to feed into our supervised machine learning model, using the K-Nearest Neighbor Classifier algorithm. The results of our machine learning model determined that The Cheesery could accurately recommend cheddar and mozzarella cheeses to customers, based on the classifying cheese categories in our dataset, but no other cheeses could be accurately recommended with the current data. Because our model focused on cheese created in Texas, the available data to provide the model is limited, e.g. if only one Texas cheesemaker sells a feta cheese, our team could not give the model more data about feta cheeses in Texas. 

---
### The Project Details

**The Communication Protocol**

<img width="421" alt="Screenshot 2022-07-20 120612" src="https://user-images.githubusercontent.com/79942792/180041510-3b7aa78c-9654-4288-834e-636596b5b1b2.png">



**Resources**

https://towardsdatascience.com/machine-learning-basics-with-the-k-nearest-neighbors-algorithm-6a6e71d01761
