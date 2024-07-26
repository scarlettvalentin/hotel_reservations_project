<img src="images/banner.png/" style="height:300px">

# Hotel Reservations
Author: [Scarlett Valentin](https://www.linkedin.com/in/scarlett-valentin/)

# Overview
The purpose of this project is to create a model to predict the number of hotel booking cancelations. This model will help hotel operations overbook hotel rooms in anticipation of cancelations, thus increasing profits of the hotel. I used the [Hotel Reservations Dataset](https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset) to create this model. The final model is a Decision Tree Classifier evaluated with 85% accuracy, 86% precision, and an AUC of 0.8. The features with the greatest importance are lead time, reservations booked online, average price per room and the number of special requests. I recommend using the decision tree classifier to predict booking cancelations and overselling approximately 87% of those rooms to avoid losing money on cancelations.

# Business Understanding
With the ease of booking and canceling hotel reservations online, **hotel cancelations and no-shows have drastically increased**. This poses a significant problem for hotel revenue. Hotels are losing out on money when there are vacant rooms due to last minute cancelations. To combat this issue, I am going to create a model that can predict when a customer is going to cancel their reservation. This will allow the hotel to overbook an appropriate number of rooms so that they are not losing out on money due to vacant rooms while also not booking more rooms than there is space for in the hotel.

# Data Understanding
The [Hotel Reservations Dataset](https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset) extracted from Kaggle contains 36,275 entries of unique bookings ranging from 2017 to 2018. There are 17 features in addition to the target variable, `booking_status`. To prepare for modeling, I use `OneHotEncoder` on the categorical variables and `StandardScaler` on the quantitative variables.

# Modeling


# Evaluation


# Conclusion
- I recommend **using a Decision Tree Classifier** with `max_depth=7`. This model can be used for predicting whether a customer will or will not cancel their hotel reservation. Once the number of expected cancelations is predicted, I would recommend **overselling approximately 87% of those rooms** to ensure the hotel does not lose money on the potential profits of those rooms.
- The biggest factor of hotel booking cancelations is lead time - the number of days between the date of booking and the arrival date. That is followed by reservations booked online, average price per room and the number of special requests. I recommend further investigating **why and how these top 4 features effect booking cancelations**. 
- I recommend experimenting with **different classifier models** to increase the precision score of the predictions. In other words, create a model with less false positives to more precisely predict the number of cancelations.

# For More Information
See the full analysis in the [Jupyter Notebook](/notebook.ipynb) or review this [presentation](/presentation.pdf/). <br>
For questions, please feel free to contact me on [LinkedIn](https://www.linkedin.com/in/scarlett-valentin/).




# Repository Structure

```
├── images
├── README.md
├── notebook.ipynb
└── presentation.pdf
```
