# QTM347-Final-Project

1. Introduction
   
  Loan defaulting is a critical problem that affects a wide range of stakeholders—from individual borrowers to corporations and government institutions. Looking from a lender’s perspective, the challenge lies in identifying high-risk borrowers in order to minimize financial loss and make data-driven lending decisions. From a borrower’s standpoint, understanding the traits that make someone more or less likely to default is essential for improving loan eligibility and financial literacy. Additionally, it is especially essential for college students like us that are looking forward in building a strong credit line. Therefore, in both cases, the ability to accurately predict loan default has tangible real-world consequences, including late fees, credit score damage, garnished wages, or frozen accounts.
  
  This problem is particularly interesting because it not only impacts individuals’ financial stability but also contributes to the health and risk exposure of broader financial systems. Solving it helps answer larger questions about credit access, responsible lending, and algorithmic fairness. There are also numerous use cases in the real world—from personal banking to credit scoring systems—making this a socially and economically relevant task.
  
  To address this issue, we treated loan default as a binary classification problem (default vs. no default). Accordingly, we implemented and compared several machine learning approaches such as:
  
  - K-Nearest Neighbors (KNN) for its simplicity and ease of interpretation.
  
  - Random Forest for its robustness, ability to handle nonlinear relationships and feature importance tracking.
  
  - Neural Networks, which are capable of modeling complex interactions within the data.
  
  These methods were chosen because they are well-suited for classification tasks and have shown strong empirical performance in similar financial prediction problems. Compared to traditional statistical methods like logistic regression, our approach provides greater flexibility, better accuracy in some cases, and the ability to model deeper feature interactions. Additionally, we benchmarked performance across these models using metrics like accuracy, precision, recall, and F1-score.
  
  Key components of our approach include thoughtful data preprocessing (Took the longest time), feature engineering, and model evaluation using cross-validation techniques. However, our approach is not without limitations. For example, imbalanced class distribution can bias the model toward predicting non-defaults (315k Vs. 75k), and more complex models like neural networks may reduce interpretability—an important factor in financial decision-making.
  
  To summarize, this project aims to bridge practical financial needs with machine learning approaches to help both lenders and borrowers make more informed decisions based on historical patterns and predictive insights.
  
3. Results:
   After running the three models, we compared the performance of three classification models—K-Nearest Neighbors (KNN), Random Forest, and Neural Networks—to predict loan default. Each model showed distinct strengths and weaknesses across key metrics such as precision, recall, and F1 score.
  
  The Neural Network model achieved the highest overall performance, with an F1 score of 0.626, precision of 0.922, and recall of 0.475. This suggests that it struck the best balance between correctly identifying defaulters and minimizing false alarms. We trained the neural network using two hidden layers (64 and 32 units), ReLU activation, and cross-entropy loss, which decreased from 0.279 to 0.247 over 22 epochs, indicating effective and stable learning.
  
  The Random Forest model was the second-best performer, with an F1 score of 0.610, precision of 0.880, and recall of 0.450. It was trained using 500 estimators, and its performance reflected a solid balance between robustness and interpretability, though it was slightly less sensitive in detecting defaulters compared to the neural network.
  
  The KNN model, though the simplest, offered a competitive recall of 0.479—the highest among the three models—with precision at 0.832 and an F1 score of 0.608. Additionally, we tested multiple values of k and selected k = 9, noting that performance remained fairly stable across values. While KNN was more prone to false positives, its strong recall makes it valuable in situations where identifying potential defaulters is a priority.
  
  In summary, while the Neural Network was the most well-rounded model in terms of overall performance, KNN stood out for its recall, and Random Forest offered a strong middle ground with good interpretability. These results highlight the trade-offs between accuracy, sensitivity, and explainability that are crucial in financial decision-making.
