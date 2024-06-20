# Practical-Application-III
 Berkeley Haas AIML - Practical Application III

 Overview: In this third practical application assignment, your goal is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) you encountered in this section of the program. You will use a dataset related to the marketing of bank products over the telephone.

Data: The dataset you will use comes from the UCI Machine Learning repository. The data is from a Portuguese banking institution and is a collection of the results of multiple marketing campaigns. The classification goal is to predict if the client will subscribe a term deposit. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. The samples were acquired over a period of more than 2 years (May 2008 to November 2010).

Understanding the features

    age - numeric
    job - Type of job/occupation - categorical
    marital - Marital status - categorical
    education - Education level - categorical
    default - has credit in default? - Binary
    balance - Average yearly balance - numeric
    housing - has housing loan? - Binary
    loan - has personal loan? - Binary
    contact - contact communication type - Categorical
    day_of_week - Last contact day of the week - Date
    month - Last contact month of year - Date
    duration - Last contact duration in seconds - numeric
    campaign - Number of contacts done during the campaign and for this client - numeric
    pdays - Number of days that passed by after the client was last contacted from a previous campaign - numeric
    previous - number of contacts performed before this campaign and for this client - numeric
    poutcome - outcome of the previous marketing campaign - Categorical
    y - outcome - has the client subscribed a term deposit? - Binary

From the comparison, it is seen that, KNN would be the best model to use with 89% Accuracy and 84% Precision

From the analysis, we can see that the following features seem to have more of an effect on the outcome

    duration : Duration of marketing calls have a positive correlation. The more time spent on the call with the customer, the more they tend to subscribe
    pdays : Number of days that passed by after the client was last contacted from a previous campaign - The less the number of days , the better is the subscription
    age - Even though the correlation is not so strong with age, still the individuals in the 40-50 category tend to subscribe more
    previous - Number of contacts performed before this campaign for this client - Decently strong correlation , the more the contact the better the subscription

