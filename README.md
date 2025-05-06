# QTM347-Final-Project

1. Introduction
Loan defaulting is a critical problem that affects a wide range of stakeholders—from individual borrowers to corporations and government institutions. Looking from a lender’s perspective, the challenge lies in identifying high-risk borrowers in order to minimize financial loss and make data-driven lending decisions. From a borrower’s standpoint, understanding the traits that make someone more or less likely to default is essential for improving loan eligibility and financial literacy. Additionally, it is especially essential for college students like us that are looking forward in building a strong credit line. Therefore, in both cases, the ability to accurately predict loan default has tangible real-world consequences, including late fees, credit score damage, garnished wages, or frozen accounts.

This problem is particularly interesting because it not only impacts individuals’ financial stability, but also contributes to the health and risk exposure of broader financial systems. Solving it helps answer larger questions about credit access, responsible lending, and algorithmic fairness. There are also numerous use cases in the real world—from personal banking to credit scoring systems—making this a socially and economically relevant task.

To address this issue, we treated loan default as a binary classification problem (default vs. no default). Accordingly, we implemented and compared several machine learning approaches such as:

- K-Nearest Neighbors (KNN) for its simplicity and ease of interpretation.

- Random Forest for its robustness, ability to handle nonlinear relationships, and feature importance tracking.

- Neural Networks, which are capable of modeling complex interactions within the data.

These methods were chosen because they are well-suited for classification tasks and have shown strong empirical performance in similar financial prediction problems. Compared to traditional statistical methods like logistic regression, our approach provides greater flexibility, better accuracy in some cases, and the ability to model deeper feature interactions. Additionally, we benchmarked performance across these models using metrics like accuracy, precision, recall, and F1-score.

Key components of our approach include thoughtful data preprocessing (Took the longest time), feature engineering, and model evaluation using cross-validation techniques. However, our approach is not without limitations. For example, imbalanced class distribution can bias the model toward predicting non-defaults (315k Vs. 75k), and more complex models like neural networks may reduce interpretability—an important factor in financial decision-making.

To summarize, this project aims to bridge practical financial needs with machine learning approaches in helping both lenders and borrowers make more informed decisions based on historical patterns and predictive insights.

