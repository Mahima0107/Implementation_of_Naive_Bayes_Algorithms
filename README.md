# Naive Bayes Algorithms

Naive Bayes is simple, fast, and surprisingly effective, especially for text-heavy or high-dimensional applications. It makes a strong baseline model—easy to train and interpret—even if its independence assumption is a simplification. Gaussian Naive Bayes is commonly used because the features are continuous and normally distributed within species.

* In this dataset There are 6 columns and 150 rows.
* Algorithm Used: Naive Bayes
* Libraries: scikit-learn, pandas, matplotlib, seaborn

🌸 Key Features & Insights
* Gaussian model for continuous features : 
Since all Iris features (sepal length/width, petal length/width) are continuous, the usual approach is Gaussian Naïve Bayes: for each class, assume each feature follows a normal distribution (with its own mean and standard deviation) and compute probabilities independently per feature.
* Petal measurements are most informative : 
Analysis shows that petal length alone yields around 86 % classification accuracy. Adding petal width boosts performance to ≈96.5 %, with little additional gain from adding sepal dimensions. 
In practice, Gaussian Naïve Bayes on all four features achieves 98% accuracy on Iris. 
* Class separability pattern : 
Setosa is nearly always perfectly separable by petal size (even by simple rule).
Versicolor and Virginica overlap more, but Naïve Bayes still separates them well using feature probability distributions.

🧠 Model Accuracy
* Gaussian Naive Bayes is highly effective on Iris, thanks to the dataset’s well-behaved, near-Gaussian-distributed features.
* When the model is both trained and tested on the full dataset (i.e. no held-out test set), Gaussian Naive Bayes achieves around 98% accuracy—with perfect accuracy on Iris-setosa and about 94% on versicolor and virginica.

🔎 Summary – Model Conclusion 
* On the Iris dataset, Gaussian Naive Bayes achieves outstanding performance—typically 98% accuracy, with nearly perfect classification of setosa and only minor confusion between versicolor and virginica. Its assumptions (Gaussian features, conditional independence) are well-matched to this dataset, and its simplicity enables fast, interpretable predictions. For datasets like Iris with distinct class separation and continuous features, Naive Bayes is an excellent baseline model.  
