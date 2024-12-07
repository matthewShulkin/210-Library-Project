# 210-Library-Project

Project: Library
    
This repository contains Python code for buidling and analyzing a library book tracking system. This project is designed to manage library operations, track borrowing patters, and predict overdue returns using machine learning

Features:

Data Generation: Create syntehtic datasets for books, borrowers, and transactions
Trend analysis: tracks monthly borrowing trends as well as seasonal borrowing patterns
Overdue return prediction: predicts the likelihood of overdue returns using a classification model. Evaluate the model with accuracy scores and classification reports

Requriements:

Python libraries:
pandas
numpy
matplotli
sklearn

Setup Instructions:
Open up codebench and run on codebench!

Usage:

1st : Generate example daata
2cnd: analyze borrowing trends
3rd:Predict Overdue returns

Key Functions:

generate_books(n): generates book data
generate_borrowers(n): generates borrower data
generate_transactions(books_df, borrowers_df, n): generates transaction data
calculate_monthly_borrowing(transactions_df): calculate borrowing trends by month
plot_borrowing_trends(monthly_borrowing): plots monthly borrowing trends
classify_late_returns(transactions_df): adds a column indicating overdue returns
train_model(X,y): trains machine learning model for overdue return predictions

Example:

To visualize borrowing trends:
monthly_borrowing = calculate_monthly_borrowing(transactions_df)
plot_borrowing_trendss(monthly_borrowing)
To predict overdue returns:
transactions_df['Late_Return'] = classify_late_returns(transasctions_df)
X_train, X_test, y_train, y_test = prepare_training_datta(transactions_df)
model=train_model(X_train,y_train)
evaluate_model(model,X_test,y_test)

