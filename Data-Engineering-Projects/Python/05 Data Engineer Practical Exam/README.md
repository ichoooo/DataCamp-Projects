# Data Engineer Certification - Practical Exam - Supplement Experiments
1001-Experiments makes personalized supplements tailored to individual health needs.

1001-Experiments aims to enhance personal health by using data from wearable devices and health apps.

This data, combined with user feedback and habits, is used to analyze and refine the effectiveness of the supplements provided to the user through multiple small experiments.

The data engineering team at 1001-Experiments plays a crucial role in ensuring the collected health and activity data from thousands of users is accurately organized and integrated with the data from supplement usage.

This integration helps 1001-Experiments provide more targeted health and wellness recommendations and improve supplement formulations.

## Task
1001-Experiments currently has the following four datasets with four months of data:
* "user_health_data.csv" which logs daily health metrics, habits and data from wearable devices,
* "supplement_usage.csv" which records details on supplement intake per user,
* "experiments.csv" which contains metadata on experiments, and
* "user_profiles.csv" which contains demographic and contact information of the users.

Each dataset contains unique identifiers for users and/or their supplement regimen.

The developers and data scientsits currently manage code that cross-references all of these data sources separately, which is cumbersome and error-prone.

Your manager has asked you to write a Python function that cleans and merges these datasets into a single dataset.

The final dataset should provide a comprehensive view of each user's health metrics, supplement usage, and demographic information.

* To test your code, your manager will run only the code `merge_all_data('user_health_data.csv', 'supplement_usage.csv', 'experiments.csv', 'user_profiles.csv')`
* Your `merge_all_data` function must return a DataFrame, with columns as described below.
* All columns must accurately match the descriptions provided below, including names.

## Data
The provided data is structured as follows:
<img width="743" height="459" alt="schema" src="https://github.com/user-attachments/assets/8f06aa5b-6d1b-47ab-a312-3cd1b93d7751" />

The function you write should return data as described below.

There should be a unique row for each daily entry combining health metrics and supplement usage.

Where missing values are permitted, they should be in the default Python format unless stated otherwise.

<img width="864" height="700" alt="image" src="https://github.com/user-attachments/assets/e246069f-d319-47b0-8c67-574b1568337d" />
