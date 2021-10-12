# Churn-Prediction

**Case Background**

Imagine TalkTel is one of the leading telecommunication providers in India. Let’s start with its product portfolio.

TalkTel has a strong presence across the country. It offers Broadband internet service that includes its fiber internet and dongle services. It also offers postpaid and prepaid plans, both in voice calls and data. It also offers DTH services under its TV packages. Other services include partnerships with OTT service providers and handset manufacturers.

All these services are also available as bundles for TalkTel’s customers. A bundle essentially is when a firm offers more than just one of its services to its customers. Its customers are present across its entire portfolio. However, in order to avoid the loss of customers, it needs to understand them better. Let’s understand what are the key metrics that govern its business?

**Problem statement**
First metric is the average revenue per user, also known as ARPU. Average revenue per user tells the story of how much money a company is making for each person using its service. It is synonymous to customer lifetime value. Generally, telecommunications companies that offer bundling services enjoy a higher ARPU.

Second metric is customer churn. Customer churn is defined in a similar fashion as you have studied throughout this program. This metric measures the number of subscribers who leave and obviously, a low churn rate is ideal. Companies that experience a high churn rate are under more pressure to generate revenue from other areas or gain new customers.

Third metric is subscriber growth rate. A telecommunications company's future revenue growth has much to do with its ability to grow its customer base and add new subscribers. Subscriber growth is, therefore, an extremely important metric. A steady subscriber growth rate indicates a competitive telecommunications company that is keeping up with technology trends, thereby keeping customers happy and attracting new customers.
Subscriber acquisition cost is very similar to customer acquisition cost. Although it seems straight-forward, subscriber acquisition cost has many layers. Of course, you’re going to need to factor in money spent on marketing and advertising. But those aren’t the only costs involved with gaining new subscribers. You also need to factor in commission costs to the people selling your product, as well as the costs involved with actually onboarding customers.
Coming to TalkTel, although the firm has a stronghold in the sector, its customers are gradually migrating to competition. If this churn doesn’t stop, the firm will be in huge trouble.
So due to intense competition and the threat of going bust, it decides to hire you as the data analyst and come up with a strategy to counter this.
As a data scientist in the marketing department of company X, help them design a program to reach a given customer at the right time with relevant offers so as to enhance its customers retention and improve client loyalty.
Do you have a quantitative approach in your mind that can predict which of their existing customers are likely to discontinue their service and should be the target audience for this campaign?
In such scenarios, you develop a model for identifying the customers who are likely to churn and should be targeted for this campaign which brings us to our next section on “Customer Churn Analysis”.

o	Perform exploratory data analysis
o	Preprocess the data
o	Select the right model.
o	Train the model
o	Test the model (Predictions and reporting)
o	Evaluate the model performance
o	Suggest ways of improving the model
Following are some points for you to take note of, while doing the assignment:
1. The data in some of the rows in the data set may be corrupted.
2. Try to simplify the code & write comments for better understanding.
3. State all your assumptions clearly.
4. Provide clear explanations to explain your stand.

**Solution Approach**

To solve this problem from Data Mining we follow the following steps
1.	Data set preparation
Import the data file provided in assignment for building classification models using Machine Learning Import dataset in using pandas and checked the dataset if there is any null value.


2.	Data collection and cleaning
i.  From check data it appears there are 11 Rows out of total 7043 (0.15%) has “null” values in total charges so these rows are removed from data sets
ii. Converted the “Total charges” and monthly charges” variable from floating to numeric type to ensure only positive charges

3.	Feature Selection & engineering
In feature selection, we analyzed the problem statement to figure that Churn is the critical factor that we need analyze from customers tenure type, contract data

4.	Exploratory Data Analysis (EDA)
In this EDA we analyzed the key trends of the Customer

5.	Model building and Model diagnostic
The model building followed the approach to divide the data into 70-30 where 70% data were used for training the model and 30% rows were used to test the model accuracy.
o	Logistic regression Model - 80.7%
o	Random forest model	- 81.3%
o	Support vector machine (SVM) – 80.9%


6.	Ways of further improvement in Model


a)	**By having mode data records**
Having more data records will lead to more data results in better and accurate models. Data records from Customer age group or other fields like “detractors” of opting other services or churn will help to analyze model more accurately and predict

b)	**Treat missing and Outlier values**
The unwanted presence of missing and outlier values in the training data often reduces the accuracy of a model or leads to a biased model. It leads to inaccurate predictions. This is because we don’t analyze the behavior and relationship with other variables correctly. As we highlighted above that 0.15% of data rows have “null” in total charges so having some assumption-based data filling or calculation done based on tenue*monthly charges to autofill the null values will improve outliers and missing values.
 
c)	**Multiple algorithms**
Selection of right algorithm is the best approach to achieve higher accuracy of model. But it is easier said than done.
This intuition comes with experience and incessant practice. Some algorithms are better suited to a particular type of data sets than others. Hence, we should apply all relevant models and check the performance.

d)	**Algorithm refining**
By refining and tuning the parameters like contract, payment type and other parameters to improve the accuracy of model. Also learning from the business perspective like what is the nature of customers from the value of monthly bills and services offered by the TalkTel company.

