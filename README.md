# Hotel-Reservation-ML-Model
## Source: https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand

### Can you predict if the customer is going to honor the reservation or cancel it?

### Business Problem: The online hotel reservation channels have dramatically changed booking possibilities and customers' behavior.  
- Reservations can get called off due to cancellations or no-shows.  Depending on the resuls, hotel managers should consider readjusting the feels that affect the reservation. 
- It would be convenient for hotels to have a model to predict if a guest will actually come. This can help hotels plan logistics, such as personal and food requirements. 
- Models that offer more rooms.
- I built a Decision Tree Classifier and KNN Machine Learning Model on making predictions of how booking was cancelled in an hotel. 

### Feature Importance
- Which features are most important to predict cancelations?



### **Content**
- This data contains booking information for a city hotel and a resort hotel.  Other features include the dates, length, parking, daily rates, and etc. 


# Insights and Visualizations 

###  Which country has the highest booking?
![Unknown](https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/f0e56b89-bb70-4afb-80a7-a8b88e2a127c)



![newplot](https://user-images.githubusercontent.com/74616874/224289458-96b52faf-6b89-4949-9d51-82160346fdda.png)
- Most of these guests are coming from Europe, mostly from Portugul.  

### Cancellation Status 
#### How many booking was canceled?
![booking canc](https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/3df03fb8-e7f6-4af8-ad7c-e933fd0d1dc8)

- It shows that City Hotel had  24,025 bookings that was cancelled compared to Resort Hotel of 28,000 bookings that was cancelled. 

#### Which month and year does Cancellation affect most?
![Unknown](https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/38d76cf6-332b-418b-94bd-bfc69c187fd1)

- 2016 has the most cancelled year of Booking in City Hotel

#### Which month and year had the most bookings?
![Unknown](https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/c0136565-9598-45b4-a045-c0a8e9533d29)

####  What are the most important columns for our prediction?
![Unknown](https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/15f65fa6-a13b-475f-9849-95b64f910f41)




# Best Metrics

## KNN Test Report
<img width="457" alt="Screen Shot 2023-09-28 at 5 38 20 PM" src="https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/95b3c5bd-3aca-4bbf-9fb2-2173fccf5115">

![Unknown](https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/f8fbd639-dc80-46a6-9652-d2fc03c8b194)

## Decision Tree Classifier 

<img width="441" alt="Screen Shot 2023-09-28 at 5 41 19 PM" src="https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/aee477f1-efe6-4dc1-8d1a-82e9a114a7b9">



# Recommendations 
1. Set up more marketing campaigns in Europe with the number of guests this region. 
2. Room H is the most popular, followed by Room G and F. Room A and B are the cheapest ones. 
![Unknown-2](https://user-images.githubusercontent.com/74616874/224291804-eecfc5cc-6215-4ae3-a425-60a55e5ed702.png)



# Code Reference 
## Functions 

### Evulate Classification
## Define a function that takes in arguments and prints out a classification report and confusion matrix
<img width="627" alt="Screen Shot 2023-09-28 at 11 35 03 AM" src="https://github.com/rimchristian/Hotel-Reservation-ML-Model/assets/74616874/489c696d-12cc-4048-af7b-f6805787db9a">

### This function takes in a model, features, and labels as arguments and prints a classification report and confusion matrix.  Has a number of operational arguments, including:
- cmap: The colormap to use for the confusion matrix.
- normalize: The confusion matrix normalization to use, or None to not normalize the confusion matrix.
- classes: An ordered list of class labels. If not specified, the class labels will be inferred from the data.
- figsize: The size of the figure to use for the confusion matrix.
 This function is a useful tool for evaluating the performance of classification models. It can be used to compare different models, or to evaluate the performance of a model on a new dataset. This specific one is used for measuring logistic regressions. 

