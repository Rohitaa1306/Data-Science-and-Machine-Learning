# Decision Trees

## Tasks

Use decision tree to perform classification to predict whether a patient has diabetes or not.

## Dataset

The Diabetes Dataset is a collection of medical data from female patients of Pima Indian heritage. The dataset contains information on various medical variables, including glucose level, blood pressure, and body mass index, and their relation to the onset of diabetes in the patients.

The dataset consists of 9 variables:

- **Pregnancies:** Number of times pregnant
- **Glucose:** Plasma glucose concentration a 2 hours in an oral glucose tolerance test
- **BloodPressure:** Diastolic blood pressure (mm Hg)
- **SkinThickness:** Triceps skin fold thickness (mm)
- **Insulin:** 2-Hour serum insulin (mu U/ml)
- **BMI:** Body mass index (weight in kg/(height in m)^2)
- **DiabetesPedigreeFunction:** Diabetes pedigree function
- **Age:** Age in years
- **Outcome:** Class variable (0 or 1) indicating whether or not the patient developed diabetes within 5 years of the initial examination. A value of 1 indicates that the patient developed diabetes, while a value of 0 indicates that they did not develop diabetes.

## The Decision Tree Algorithm

Decision tree is a supervised learning algorithm used for classification and regression tasks. It is a type of model that learns simple decision rules from the data and builds a tree-like structure to represent the decision-making process.

### The idea behind decision tree:

The idea behind decision tree is to recursively split the data into subsets based on the values of the input features such that the target variable is more homogeneous within each subset. This is done by choosing the feature that maximizes the information gain, which is a measure of the reduction in uncertainty about the target variable after the split. The split is continued until a stopping criterion is met, such as a maximum depth of the tree or a minimum number of samples required to split a node.

### The decision tree structure:

The decision tree can be represented as a flowchart-like structure where each internal node represents a test on an input feature, each branch represents the outcome of the test, and each leaf node represents a class label or a regression value. The decision rule at each internal node is simply a threshold on the input feature, and the decision boundary between two classes is a hyperplane perpendicular to the feature axis.

##Conclusion
Overall, the decision tree is a powerful and interpretable algorithm that can handle both categorical and numerical input features and can capture complex nonlinear relationships between the input features and the target variable. However, it is prone to overfitting when the tree is too deep or when the training set is too small, and it may fail to capture interactions between different input features. Therefore, it is often used in ensemble methods such as random forests or boosting to improve its performance and robustness.
