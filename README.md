# Telecom-Churn-Analysis---Capstone-Project

Telecom Churn Analysis - Capstone Project
## <b> Orange S.A., formerly France Télécom S.A., is a French multinational telecommunications corporation. The Orange Telecom's Churn Dataset, consists of cleaned customer activity data (features), along with a churn label specifying whether a customer canceled the subscription.

## <b> Goal :Explore and analyze the data to discover key factors responsible for customer churn and come up with ways/recommendations to ensure customer retention. </b>

![download (5)](https://user-images.githubusercontent.com/73479133/202292221-1f52c9a4-a525-43eb-a56e-ca659c29e64b.png)

<p><img alt="Insight logo" src="https://drive.google.com/uc?export=view&id=1q12QkUJV93coNY1p2iQV15UHxfkH4na0" align="left" hspace="25px" vspace="20px" width="40" height="50" ></p>

#What is customer churn?

Customer churn is the term used when an existing customer stops using a company’s services and/or stops buying their products. In other words, the customer chooses to cut his ties with the company. 

![download](https://user-images.githubusercontent.com/73479133/202292282-6e6795cb-fdaa-4a69-ab5e-663c9986fe2a.gif)

# **Customer churn rate** 
 is defined as the proportion of customers who
stopped using a particular company’s products or services during
a definite time frame.
<br/>
<br/>

Mathematically


<br/>

\begin{align}
        \text{C(T)} = \frac{\text{A(T)}}{\text{B(T)}} \times 100
    \end{align}



where,

**C** represents the churn % for a time frame T,

**A(T)** represents the total number of customers after time T,

**B(T)** represents the total number of customers before time T.



<p><img alt="Insight logo" src="https://drive.google.com/uc?export=view&id=1pNPWpgMSrFyFEo7TLhqOZXnSTicDLHLe" align="left" hspace="10px" vspace="10px" width="55" height="65" ></p>


# All features

* **State:** 51 Unique States in United States of America

* **Account Length:**  Length of The Account

* **Area Code :** 3 unique codes, 408 is of San Jose, 415 is of San Francisco and 510 is of City of Okland

* **International Plan:** Yes Indicate International Plan is Present and No Indicates no subscription for Internatinal Plan

* **Voice Mail Plan:** Yes Indicates Voice Mail Plan is Present and No Indicates no subscription for Voice Mail Plan

* **Number vmail messages:** Number of Voice Mail Messages ranging from 0 to 51.

* **Total day minutes:** Total Number of Minutes Spent By Customers in Morning

* **Total day calls:** Total Number of Calls made by Customer in Morning.

* **Total day charge:** Total Charge to the Customers in Morning.

* **Total eve minutes:** Number of Minutes Spent By Customers in Evening

* **Total eve calls:** Total Number of Calls made by Customer in Evening.

* **Total eve charge:** Total Charge to the Customers in Evening.

* **Total night minutes:** Total Number of Minutes Spent By Customers in the Night.

* **Total night calls:** Total Number of Calls made by Customer in Night.

* **Total night charge:** Total Charge to the Customers in Night.

* **Total intl minutes:** Total Number of Minutes Spent By Customers in international calls.

* **Total intl calls:**  Total Number of International calls made by Customer.

* **Total intl charge:** Total charge to Customers in international calls.

* **Customer service calls:** Total number of Calls by Customer to service Center, ranging from 0 to 9.

* **Churn:** Whether he customer churned or not(True or False).


<p><img alt="Insight logo" src="https://drive.google.com/uc?export=view&id=14dpaeXX-ajsM8quwe3dCCdQdrdvf29iI" align="left" hspace="20px" vspace="20px" width="45" height="60" ></p>

#**Overall Conclusion**

---

1. **Observation 1**
  * 14.5% of Orange Telecom's customers have churned, from a customer churn perspective it's still high.Our job will be to reduce it as much as possible.

2. **Observation 2**
  * Charges for International calls are highest, followed by day, then evening and night calls are cheapest.
  * On average, our customers prefer to talk more at night and evening than during the day.

3. **Observation 3**
  * Most of the feature approximately follows Normal Distribution, means most of the values centered around mean of the distribution. As we move away from centre their value count gradually decrease.
  * Most people don't send any voicemails.
  * The graph of total international calls and Customer service calls are positively skewed.

4. **Observation 4**
  * Number of Voice mail is highly correlated with voice mail plan.
  * Total day minutes is perfectly correlated with total day charge, and it follows same pattern in evening, nights minutes and international minutes with charges.

  **Churn Lable have**

  * Positive correlation with
    * International plan, means for those users who have taken the international plan, there is a high chance of getting churned.
    * Customer service calls,If the customer makes more service calls, the chances of churn are also higher.
    * Total day minutes is also positivly correlated, we will further explore it.

  * Negative correlation with
    * Voice mail plan, means for those users who have taken the Voice mail plan, then chance of getting churn will reduce.
    * We have already seen that, if person has a voicemail plan, only then s(he) sends voicemail.

  * Almost zero  correlation with

    * Account length, Area code and total calls at any time.

5. **Observation 5**

  * As we can see that Account length, Area code, total calls at different time does not affect the churn behavior of the customers.
  * Area code 415 has twice as many customers as others.

6. **Observation 6**

  **Customers are not satisfied with international plans**
    * The Churn rate of customers who have taken international plans is much higher than average.
    * Customers who did not take international plan also make international calls but their churn rate is normal.

7. **Observation 7**

 * It seems that customer are satisfied with voice mail plan.

 * Voicemail plan unable to satisfy all types of customers, those who send more vmails

8. **Observation 8**

  * We have noticed that the charges are higher during day time as compared to evening and night, this is the first reason for customer dissatisfaction.

9. **Observation 9**

 * Churn rate increases significantly for 4 or more calls to the customer service.

 * Customers who talk less in a day (below 200) do not churn so easily until their problem is solved, they are trying to solve their problems by talking to the service center as much as possible, even after that if their problems are not resolved then they churn.

  * Customers who talk more during the day have higher churn rate even in low service calls, means they are not happy high call rate in day.

10. **Observation 10**
  * Churn rate is very high in few state like  New Jersey, california, Texas etc.


11. **Observation 11**

  * In reduced dimensions, dissatisfied customers are grouped together, same dissatisfaction was observed in group, users that are not satisfied by particular policy are Churning together.
  
  
  # **Recommendations**
----
For  Churn Prevention: How to retain your customers

![download (6)](https://user-images.githubusercontent.com/73479133/202292575-eacb8510-0c06-4acc-b7d6-c4094d7cd096.png)


Many customers do international conversations, but most of them have not taken any international plan, which means they dislike our international plan.
And those who have taken it, their churn rate is very high.

# First Suggestion
* **We need a very attractive international plan, which can provide satisfaction to the customers making international calls.**

---
___

By the way, the customer who has taken the voicemail plan has seen a lower Churn rate, which means that our voicemail plan is good, But customers who send more voicemails have seen higher churn rates.

# Second Suggestion 

* **We need a new voice mail plan along with the old one which is specially designed keeping in mind the more voicemail senders.**

---
---

We noticed that people who call customer service more than 3 times, their churn rate is drastically increased, means despite calling the service center so many times, their problem could not be solved.

# Third Suggestion

* **Need to improve the feedback system that doesn't ignore customer problems**
___
---
We noticed that the call rate of the day is high, so the customers who talk more during the day have seen higher churn rate than others.
They have higher churn rate even in  service calls  less than 3, means they do not like any of our day's  plans, they do not want to listen to any excuses.

# Fourth Suggestion


* **Need to introduce better tariff plans for day calling which is specially designed for users to talk too much in a day.**

____
____

The churn rate has also been seen high among the callers in the evening, but it is less than the day.

# Fifth suggestion

* **Therefore, there is a need for improvement in the evening tariff plans as well**,
----
----

In the states where the churn rate is more than 20, there is a slight dislike for the night calls.

# Sixth suggestion

* **The company can launch better night calls tariff which is specifically designed for specific states.**
