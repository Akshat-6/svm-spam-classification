# svm-spam-classification
SVM classification with decision boundary visualization before and after feature scaling using a spam classification dataset.

📧 SVM Spam Classification – Performance & Visualization
This project demonstrates the use of Support Vector Machine (SVM) for spam classification using a dataset with email features. It compares the model's performance before and after feature scaling and visually presents the decision boundary for clear understanding.

📌 Objective
Build an SVM classifier to detect spam emails.

Visualize the model’s classification and decision boundary.

Understand the impact of feature scaling on SVM performance.

📁 Dataset
File: spam_classification_dataset.csv

Features:

Email_Length

Hyperlinks

Keyword_Frequency

Special_Characters

Target:

Is_Spam (0 = Not Spam, 1 = Spam)

🛠️ Steps Performed
✅ 1. Import Libraries
Libraries used: pandas, numpy, matplotlib, seaborn, sklearn

✅ 2. Load and Explore Dataset
Loaded CSV into a DataFrame

Used sns.pairplot() and sns.heatmap() for visual EDA

✅ 3. Data Preparation
Split into features X and target y

Train-test split using train_test_split(test_size=0.2)

Feature scaling using StandardScaler

✅ 4. Train the SVM Model
Trained SVM using SVC(kernel='linear') on scaled data

Accuracy evaluated using accuracy_score

✅ 5. Visualization of Decision Boundary
Selected first 2 features: Email_Length, Hyperlinks

Trained a new SVM on these for 2D visualization

Created meshgrid and plotted decision boundary using contourf and scatter

📊 Results
Without Scaling: Lower accuracy and poorly defined decision boundary.

With Scaling: Improved accuracy and cleaner separation between classes.

Visuals: 2D plots clearly show decision boundaries for both cases.

💻 Libraries Used
Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

🚀 Future Work
Try RBF and polynomial kernels for improved performance.

Apply PCA for visualizing all features in 2D.

Tune hyperparameters using GridSearchCV.


