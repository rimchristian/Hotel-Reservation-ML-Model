# Hotel-Reservation-ML-Model
## Source: https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand

###**Can you predict if the customer is going to honor the reservation or cancel it?**

### **Business Problem: The online hotel reservation channels have dramatically changed booking possibilities and customers' behavior.  
Reservations can get called off due to cancellations or no-shows.  Depending on the resuls, hotel managers should consider readjusting the feels that affect the reservation. 
Some of the questions that can be answered is the best time to book a hotel room? The optimal length of stay in order to get the best daily rate?

### **Content**
- This data contains booking information for a city hotel and a resort hotel.  Other features include the dates, length, parking, daily rates, and etf. 


# Insights

### The top 5 places most guests are coming from: 
**Country** | **# of Guests**  
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

