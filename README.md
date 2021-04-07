# Telecom_Churn
Problem statement:
Business Problem Overview
In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.

For many incumbent operators, retaining high profitable customers is the number one business goal.

To reduce customer churn, telecom companies need to predict which customers are at high risk of churn.

In this project, customer-level data of a leading telecom firm is analysed for building predictive models for identifying customers at high risk of churn and also to identify the main indicators of churn.

Business Objective:
The dataset provided for Indian and Southeast Asian market contains customer-level information for a span of four consecutive months - June, July, August and September. The months are encoded as 6, 7, 8 and 9, respectively.

The business objective is to predict the churn in the last (i.e. the ninth) month using the data (features) from the first three months. To do this task well, understanding the typical customer behaviour during churn will be helpful.
Some Important points for Churn -
In the postpaid model, anticipating churn instance from customers is easy as when customers want to switch to another operator, they usually inform the existing operator to terminate the services. However, in the prepaid model, predicting churn is usually more critical (and non-trivial). In this case customers who want to switch to another network can simply stop using the services without any notice, and it is hard to know whether someone has actually churned or is simply not using the services temporarily. Prepaid is the most common model in India and southeast Asia

-- Broadly churn can be defined in two ways:

Revenue-based churn: Customers who have not utilised any revenue-generating facilities such as mobile internet, outgoing calls, SMS etc. over a given period of time.

Usage-based churn: Customers who have not done any usage, either incoming or outgoing - in terms of calls, internet etc. over a period of time. In this study this type of churn will be used.

-- High-value Churn:

In the Indian and the southeast Asian market, approximately 80% of revenue comes from the top 20% customers (called high-value customers). Thus, reducing churn of the high-value customers, will reduce significant revenue leakage. In this study churn will be predicted only on high-value customers.

-- Customer Behaviour During Churn:

In churn prediction, we assume that there are three phases of customer (especifically for high-value customer) lifecycle:

1 The ‘good’ phase - Here the customer is happy with the service and behaves as usual.

2 The ‘action’ phase - The customer experience starts to sore in this phase, for e.g. he/she gets a compelling offer from a competitor, faces unjust charges, becomes unhappy with service quality etc. In this phase, the customer usually shows different behaviour than the ‘good’ months. Also, it is crucial to identify high-churn-risk customers in this phase, since some corrective actions can be taken at this point (such as matching the competitor’s offer/improving the service quality etc.)

3 The ‘churn’ phase - In this phase, the customer is said to have churned. Here churn will be defined based on this phase. Also, it is important to note that at the time of prediction (i.e. the action months), this data is not available for prediction. Thus, after tagging churn as 1/0 based on this phase,all data corresponding to this phase to be discarded.

In this case, since this study is being done over a four-month window, the first two months are the ‘good’ phase, the third month is the ‘action’ phase, while the fourth month is the ‘churn’ phase.
