# credit-risk-classification

OVERVIEW

Machine Learning Model 1:
The logistic regression model is really good at figuring out which loans are safe (0) and which are risky (1). Here's a quick rundown of how well it does:

The aim of this analysis is to create a predictive tool for a peer-to-peer lending platform, focusing on distinguishing between low-risk and high-risk loans using historical data. This effort is key for lenders to lower the risk of defaults and make informed decisions about loan approvals.

We analyzed a dataset detailing borrowers' financial backgrounds, including credit scores, loan amounts, and income, to predict the likelihood of loan default (high risk) or repayment (low risk).

Workflow Highlights:

Preparation: Processed the data, isolating the key variable ('loan_status') from other influencing factors.
Splitting: Divided the dataset for training and testing, ensuring the model could be validated against new data.
Modeling: Chose logistic regression for its simplicity and effectiveness in binary outcomes prediction.
Evaluation: Assessed the model's accuracy with basic metrics, focusing on its ability to correctly classify loan risk.
Key Techniques:

Logistic Regression: Ideal for predicting binary outcomes, providing insights into the probability of each classification.
Train-Test Split: Essential for testing model performance on unseen data.
Metrics: Used to evaluate the model's success in predicting loan risk, including precision, recall, and F1-scores.

THE RESULTS

For Safe Loans (0):

Precision: Perfect score of 1.00! This means it hardly ever makes a mistake, misclassifying very few of the 18,761 loans. Recall: Also a perfect 1.00! It catches almost all the safe loans, hardly missing any. For Risky Loans (1):

Precision: Scores 0.87, so when it says a loan is risky, it's right 87% of the time. Recall: Gets a 0.92, finding 92% of the actual risky loans. Only a tiny bit slips through the cracks out of 623. Balanced Accuracy Score: Stands at 0.96, showing it's really good at handling both loan types, even though there are way more safe loans than risky ones.

F1-Scores: Nails a perfect 1.00 for safe loans and a strong 0.90 for risky ones, proving it's on point.

Overall Accuracy: Hits 0.99, meaning 99% of its guesses are spot on, which is pretty awesome.

Looking at the Numbers:

Nails identifying 18,761 safe loans. Spots 563 risky loans correctly. Mistakenly flags 102 safe loans as risky. Misses spotting 56 risky loans. This easy look at the numbers shows how great the logistic regression model is at telling apart safe and risky loans, making it super useful for figuring out loan risk.

Machine Learning Model 2:
The logistic regression model, after being adjusted with oversampled data, showcases remarkable effectiveness in distinguishing between safe and risky loans. Let's break down its performance:

Balanced Accuracy Score: Achieves an impressive 0.996, highlighting the model's exceptional ability to equally predict both loan categories accurately.

Confusion Matrix:

Correctly identifies 18,670 safe loans while misclassifying only 91 as risky. Excellently detects 621 out of 623 high-risk loans, with a minimal 2 misclassified as safe. Precision:

For safe loans, it's practically perfect, ensuring almost no safe loans are incorrectly marked as risky. Risky loans have a precision of 0.87, meaning that when the model predicts a loan as risky, it's correct about 87% of the time. Recall:

Nearly flawless for safe loans, missing almost none. Perfect for risky loans at 1.00, capturing every actual high-risk loan. F1-Score:

Safe loans get a perfect score of 1.00, indicating excellent precision and recall balance. Risky loans score a 0.93, showing a strong balance between precision and recall, emphasizing the model's accuracy in identifying high-risk loans. Overall Accuracy: Stands at a stellar 1.00, showcasing the model's reliability in accurately classifying both healthy and high-risk loans.

This concise overview demonstrates the logistic regression model's superior performance, particularly its flawless recall for high-risk loans, proving the effectiveness of oversampling in combating class imbalance.

SUMMARY

Both models excel in assessing loan risk, yet they exhibit minor differences:

Model 1 showcases exceptional precision in identifying both safe and high-risk loans, achieving nearly perfect metrics and 99% accuracy overall. It excels in detecting safe loans and performs well with risky ones too.

Model 2 edges out slightly in handling the imbalance between safe and risky loans, maintaining near perfect accuracy and showing a particular strength in pinpointing high-risk loans.

Recommendation

Opt for Model 2 if prioritizing the identification of risky loans is key. Its enhanced ability to discern such loans makes it ideal for minimizing defaults and optimizing risk management.
