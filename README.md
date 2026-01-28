Model Choice Justification: CatBoost Classifier

In this project, CatBoostClassifier was selected as the final and only model for loan approval prediction.

Why CatBoost?

Native handling of categorical features: CatBoost efficiently processes categorical variables without requiring extensive one-hot encoding, reducing information loss.

Strong performance on small and imbalanced datasets: The dataset size is limited, and CatBoost is known to perform well in such scenarios due to ordered boosting.

Reduced overfitting: Its built-in regularization and symmetric tree structure help control overfitting.

Minimal preprocessing required: Compared to other gradient boosting models, CatBoost requires fewer manual feature transformations.

Performance Justification

CatBoost achieved an accuracy of ~83% with a strong F1-score, especially improving recall for approved loan cases while maintaining reasonable performance on rejected cases. This balance makes it suitable for real-world financial decision systems where false negatives are costly.

Production Readiness

Using a single, stable model simplifies:

Model monitoring

Version comparison in the model registry

Logic-gate based deployment decisions

This aligns well with MLOps best practices, where consistency and reliability are preferred over unnecessary model complexity.

