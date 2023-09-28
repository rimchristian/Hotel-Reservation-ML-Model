# Hotel-Reservation-ML-Model
## Source: https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand

### Can you predict if the customer is going to honor the reservation or cancel it?

### Business Problem: The online hotel reservation channels have dramatically changed booking possibilities and customers' behavior.  
- Reservations can get called off due to cancellations or no-shows.  Depending on the resuls, hotel managers should consider readjusting the feels that affect the reservation. 
- It would be convenient for hotels to have a model to predict if a guest will actually come. This can help hotels plan logistics, such as personal and food requirements. 
- Models that offer more rooms. 

### Feature Importance
- Which features are most important to predict cancelations?



### **Content**
- This data contains booking information for a city hotel and a resort hotel.  Other features include the dates, length, parking, daily rates, and etc. 


# Insights

### The top 5 places most guests are coming from: 
**Country** | **Number of Guests**  
--- | ---
Portugul | 17572 
Great Britain | 8440
France | 7091
Spain | 5382
Deutch | 4332


![newplot](https://user-images.githubusercontent.com/74616874/224289458-96b52faf-6b89-4949-9d51-82160346fdda.png)
- Most of these guests are coming from Europe, mostly from Portugul.  

### Cancellation Status 
![Unknown](https://user-images.githubusercontent.com/74616874/224290741-ace62c93-9947-445f-b948-02cc9c66b4a1.png)
- The two classes were not distributed balanced so the data may be imbalanced. 1 for Canceled and 0 for Not Canceled. I will try to balance the classes. 

# Best Metrics
CLF Report               precision    recall  f1-score   

           0       0.95      0.95      0.95     15767
           1       0.87      0.87      0.87      5928

    accuracy                           0.93     21695
   macro avg       0.91      0.91      0.91     21695
weighted avg       0.93      0.93      0.93     21695

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

