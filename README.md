# Predicting churn

The gym chain Model Fitness is developing a customer interaction strategy based on analytical data.
One of the most common problems gyms and other services face is customer churn. For a gym, it makes sense to say a customer has left if they don't come for a month. Of course, it's possible they're in Cancun and will resume their visits when they return, but's that's not a typical case. Usually, if a customer joins, comes a few times, then disappears, they're unlikely to come back.
In order to fight churn, Model Fitness has digitized a number of its customer profiles. Your task is to analyze them and come up with a customer retention strategy.

You should:
- Learn to predict the probability of churn (for the upcoming month) for each customer
- Draw up typical user portraits: select the most outstanding groups and describe their main features
- Analyze the factors that impact churn most
- Draw basic conclusions and develop recommendations on how to improve customer service:
    - Identify target groups
    - Suggest measures to cut churn
    - Describe any other patterns you see with respect to interaction with customers
    


## Description of the data

- 'Churn' — the fact of churn for the month in question (1- customer left, 0- customer stayed)
- Current dataset fields:
    - User data for the preceding month
        - 'gender' (1- female, 0- male)
        - 'Near_Location' — whether the user lives or works in the neighborhood where the gym is located (1- near, 0-not near) 
        - 'Partner' — whether the user is an employee of a partner company (the gym has partner companies whose employees get discounts; in those cases the gym stores information on customers' employers) (1-employee of a partner, 0-not)
        - Promo_friends — whether the user originally signed up through a "bring a friend" offer (1- they used a friend's promo code when paying for their first membership, 0- they did not)
        - 'Phone' — whether the user provided their phone number (1- provided phone number, 0- did not)
        - 'Age'
        - 'Lifetime' — the time (in number of months) since the customer first came to the gym
- Data from the log of visits and purchases and data on current membership status
    - 'Contract_period' — 1 month, 3 months, 6 months, or 1 year (in number of months)
    - 'Month_to_end_contract' — the months remaining until the contract expires (in number of months)
    - 'Group_visits' — whether the user takes part in group sessions (1-takes part in group sessions, 0-does not)
    - 'Avg_class_frequency_total' — average frequency of visits per week over the customer's lifetime
    - 'Avg_class_frequency_current_month' — average frequency of visits per week over the preceding month
    - 'Avg_additional_charges_total' — the total amount of money spent on other gym services: cafe, athletic goods, cosmetics, massages, etc.
