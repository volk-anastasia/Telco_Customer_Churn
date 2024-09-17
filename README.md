# Telco Customer Chun
[Kaggle dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

**GOAL:** predict behavior to retain customers.  

---
## Architecture


#### EDA

The features:
1. gender (Male, Female)
2. SeniorCitizen (Yes, No)
3. Partner (Yes, No)
4. Dependents (Yes, No)
5. tenure
6. PhoneService (Yes, No)
7. MultipleLines (Yes, No, No phone service)
8. InternetService (DSL, No, Fiber optic)
9. OnlineSecurity (Yes, No, No internet service)
10. OnlineBackup (Yes, No, No internet service)
11. DeviceProtection (Yes, No, No internet service)
12. TechSupport (Yes, No, No internet service)
13. StreamingTV (Yes, No, No internet service)
14. StreamingMovies (Yes, No, No internet service)
15. Contract (Month-to-month, One year, Two year)
16. PaperlessBilling (Yes, No)
17. PaymentMethod (Bank transfer (automatic), Mailed check, Electronic check, Credit card (automatic))
18. MonthlyCharges
19. TotalCharges
20. Churn

![image](https://github.com/user-attachments/assets/1d0fa4a1-fba2-4a26-aaa6-06075a3cb41d)

- `gender` - gender does not affect the client's decision
- `Senior Citizen` - older people are more likely to refuse services
- `Partner` & `Dependents` - clients in relationships, as well as clients with children, are less likely to refuse services. Perhaps the company will present favorable family tariffs
- `InternetService` - customers with fiber optic more often refuse services. Customers who do not use the Internet very rarely refuse
- `OnlineSecurity`, `OnlineBackup` & `DeviceProtection` - clients who use protection systems, as well as those who use cloud storage, are more likely to refuse. Competitors also have favorable package offers with additional services
- `TechSupport` -  customers who do not contact technical support are more likely to refuse
- `Contract` - logical, clients with a short-term contract leave more often
- `PaperlessBilling` & `PaperlessBilling` - customers who receive and pay bills in a conservative way are less likely to change service providers
- Clients who have about 3-6 services most often churn.

### CatBoost
