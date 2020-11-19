# Project Three Customer Churn for SyriaTel

[Slides and Presentation Folder](https://drive.google.com/drive/folders/1NddLHopNLhAqZx7mU4sF_FbB-gEAjrpo?usp=sharing)


### Strategic Approach

The stakeholder, SyriaTel, is a telecommunications company whose goal is to better understand what factors are causing customer churn. Due to limits on data size, the model will only be robust enough to be used by SyriaTel to analyze their specific data provided.

By exploring typical customer churn and using the CRISP-DM framework, I will seek to answer the following questions: 

1. What features of the dataset are primary determinants of customer churn and to what extent?

2. What are the ways that these findings can be interpreted and how can SyriaTel implement cost-effective solutions?

3. Will these solutions be feasible in reducing the customer churn rate by at least 7%?


### The Data

The data used was provided by SyriaTel at this address: https://www.kaggle.com/becksddf/churn-in-telecoms-dataset


### Question One

[Question One Notebook Link](https://github.com/jaykayso/dsc-mod-3-project-v2-1-onl01-dtsc-ft-041320/blob/master/notebooks/Question%20One.ipynb)

Question 1: What features of the dataset are primary determinants of customer churn and to what extent?
    
I optimized for recall value which can be interpreted as optimizing against the occurences of not acknowledging a customer who is at risk of churn. Many models were explored, but the most successful was XGBoost with GridSearchCV.
    
The most influential feature findings through the exploration of SHAP values were: 

#### Contributors of High Customer Churn: Value of One

- High total number of day minutes
- High number of customer service calls
- Customers who have an international plan
- High number of night minutes
- High number of international minutes

#### Contributors of Low Customer Churn: Value of Zero

- Customers with a voicemail plan
- Customers with higher number of voicemails
- High number of international calls
    
### Conclusion

In conclusion, it seems that SyriaTel could be losing customers due to rates that fluctuate from month to month. If this is the case, a flat monthly fee with a contract would be a better business model for acquiring customers.

### Question Two

[Question Two Notebook Link](https://github.com/jaykayso/dsc-mod-3-project-v2-1-onl01-dtsc-ft-041320/blob/master/notebooks/Question%20Two.ipynb)

Question 2: What are the ways that these findings can be interpreted and how can SyriaTel implement cost-effective solutions?

The high number of minutes leading to customer churn in total day minutes and night minutes makes it obvious that customers who are using more minutes are having to pay more and therefore, looking elsewhere for more cost-effective solutions. Another concept to explore here is whether or not the customers have a contract or are simply paying month-to-month.


### Conclusion

The customers with an above average number of day minutes have been linked to being likely to churn. There are 293 of them. SyriaTel needs to reduce churn by 247 customers annually. By offering customers plans with flat monthly fees, SyriaTel will be able to reduce this churn and potentially save over $25,000.

### Question Three
    
[Question Three Notebook Link](https://github.com/jaykayso/dsc-mod-3-project-v2-1-onl01-dtsc-ft-041320/blob/master/notebooks/Question%20Three.ipynb)
    
Question 3: Will these solutions be feasible in reducing the customer churn rate by at least 7%?

The revenue by customer, not including customers with international plans was $60 on average. This does not seem like a feasible amount to charge a customer for a monthly phone subscription. 
    
### Conclusion
    
In conclusion, SyriaTel could definitely reduce churn by at least 7% if it found a way to make a subscription model profitable. 

    
# Conclusion

SyriaTel can significantly improve it's churn rate by implementing a flat monthly fee subscription model for it's customers. Not only do customers prefer subscription models as a way to automate their lives but also, subscription models help the companies using them too:
 - Customers are not upset or surprised by their bills. 
 - Companies know ahead of time what their estimated revenue is from subscriptions.
 - Companies are able to provide better solutions for unique needs of customer segments. 
 - Companies are able to build penalties around particular plans and subscriptions. 
 - When customers receive penalties they are more likely to take responsibility since they are aware of the penalties of their subscription. 
 
### Additional Recommendations: 

- Initiating customer feedback surveys for customer service calls.
- Initiating customer feedback surveys for customers leaving. This could be a requirement of cancellation via online survey or in person. 


# Future Work

Future work could allow for more customer segmenting, understanding the data in a better way and learning the answers to many of the questions posed by our findings that would be explained by understanding SyriaTel's business model. 

    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    