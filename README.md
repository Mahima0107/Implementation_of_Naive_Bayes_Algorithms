# Naive Bayes Algorithms

Naive Bayes is simple, fast, and surprisingly effective, especially for text-heavy or high-dimensional applications. It makes a strong baseline model—easy to train and interpret—even if its independence assumption is a simplification. Gaussian Naive Bayes is commonly used because the features are continuous and normally distributed within species.

* In this dataset There are 6 columns and 150 rows.
* Algorithm Used: Linear Regression
* Libraries: scikit-learn, pandas, matplotlib, seaborn

🌸 Key Features & Insights
* Gaussian model for continuous features
Since all Iris features (sepal length/width, petal length/width) are continuous, the usual approach is Gaussian Naïve Bayes: for each class, assume each feature follows a normal distribution (with its own mean and standard deviation) and compute probabilities independently per feature.
* Petal measurements are most informative
Analysis shows that petal length alone yields around 86 % classification accuracy. Adding petal width boosts performance to ≈96.5 %, with little additional gain from adding sepal dimensions. 
In practice, Gaussian Naïve Bayes on all four features achieves ≈96 %–97 % accuracy on Iris. 
* Class separability pattern
Setosa is nearly always perfectly separable by petal size (even by simple rule).
Versicolor and Virginica overlap more, but Naïve Bayes still separates them well using feature probability distributions.
