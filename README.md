# Cust_analysis-and-Predict_modeling
Explore customers reviews, gain a comprehensive understanding of passenger experience and priorities. Define key factors influencing booking patterns. Predicting Customer Booking Completions

# Objective:

The primary objective of this project is twofold:

  1.	Analyze customer reviews to identify key themes and sentiment trends that influence customer satisfaction.
	2.	Develop a predictive model that accurately determines whether a customer will complete a flight booking.

 # Data:
 	•	Customer Reviews: Textual data capturing customer feedback and experiences.
	•	Numerical features: num_passengers, purchase_lead, length_of_stay, flight_hour, flight_duration
	•	Categorical features: sales_channel, trip_type, flight_day, route, booking_origin, wants_extra_baggage, wants_preferred_seat, wants_in_flight_meal
	•	Target variable: booking_complete (whether the booking was completed)

 # Steps and Methodology:

1. Customer Review Analysis:
	•	Text Preprocessing: Standardized text data by converting to lowercase, removing special characters, and tokenizing.
	•	Sentiment Analysis: Used TextBlob to calculate sentiment polarity for each review, categorizing them into positive, negative, or neutral.
	•	Keyword Analysis: Identified the frequency of key terms such as “service,” “seat,” “crew,” “food,” etc., to understand common themes in customer feedback.

  2. Data Cleaning and Preprocessing:
	•	Removed missing values and duplicates to ensure data quality.
	•	Encoded categorical variables using OneHotEncoder and scaled numerical features using StandardScaler.
	
 3.	Feature Engineering:
	•	Extracted relevant features and created additional features based on domain knowledge.
	•	Addressed class imbalance using techniques such as SMOTE and class weights.
	
 4.	Model Training:
	•	Split the dataset into training and testing sets.
	•	Trained a RandomForestClassifier due to its ability to handle complex interactions and output feature importance.
	
 5.	Model Evaluation:
	•	Evaluated the model using accuracy, precision, recall, and F1-score.
	•	Identified that the model had high accuracy but was biased towards the majority class.
	
 6.	Feature Importance Analysis:
	•	Analyzed the feature importance to understand the most influential factors affecting booking completions.
	•	Identified key features such as purchase_lead, flight_hour, length_of_stay, and flight_duration.

7. Insights and Recommendations:
	•	Provided actionable insights based on feature importance analysis.
	•	Recommended strategies to improve booking completions, such as encouraging advanced bookings, optimizing flight schedules, and targeting group bookings.

# Key Findings:

	•	Purchase Lead: Customers who book further in advance are more likely to complete their bookings.
	•	Flight Hour: The time of the flight plays a significant role in booking completions.
	•	Length of Stay: Longer stays are associated with higher completion rates.
	•	Flight Duration: The total flight duration impacts customer decisions.
	•	Geographical Factors: Booking origins from certain countries influence completion rates.
	•	Additional Services: Preferences for in-flight meals and extra baggage are indicators of booking completion likelihood.

# Conclusion:

By leveraging the predictive model and understanding the factors influencing booking completions, the airline can implement targeted strategies to enhance customer satisfaction and increase the likelihood of booking completions. This project demonstrates the power of machine learning in deriving actionable insights from data and improving business outcomes.
