# Data Science Mini Projects

A collection of small, exploratory data science projects created during my data science studies. This repository is my learning space: a place to document experiments, practice end-to-end workflows, and build a record of the skills I am developing one project at a time.

I currently work as a **physics teacher** and am working toward a transition into **data science and AI engineering**. Teaching physics has given me a strong interest in analytical thinking, mathematical reasoning, and understanding patterns in data. I am now applying that mindset to programming, data analysis, visualization, and machine learning.

These are **mini-projects, not production systems**. The topics and techniques will vary as I explore different areas of data science. Some projects may be exploratory data analysis; others may involve statistical methods, visualization, or machine learning. The goal is to learn, experiment, reflect, and steadily improve.

---

## Projects

### 1. Personality Classification from Social Media Behavior

This project explores whether social-media behavior features can be used to classify a user into one of two dataset labels: **Introverted (0)** or **Extroverted (1)**.

The dataset contains **100 records** and includes six numerical features—posting frequency, post interactions, time spent on social media, response time, post length, and number of friends/followers—along with one categorical feature describing the most common interaction type.

The notebook walks through an introductory machine learning workflow, from understanding and preparing the data to comparing and evaluating classification models.

---

## Workflow: From Data to Model Evaluation

The first notebook follows this basic pipeline. It is a practical learning workflow for this project, not a rule that every future project in the repository must follow.

1. **Understand the data**  
   Load the CSV, inspect the available variables, identify the target, and consider how each feature may relate to the classification task.

2. **Explore and visualize**  
   Examine the numerical and categorical features. Check for missing values and potential outliers, and use plots to get a better view of the data before modeling.

3. **Preprocess the features**  
   - Use **One-Hot Encoding** for the categorical feature.
   - Use **StandardScaler** to standardize numerical features.
   - Check missing-value counts and use visualizations such as boxplots to inspect the data.

4. **Explore dimensionality and structure**  
   - Apply **Principal Component Analysis (PCA)** to examine explained variance and feature contributions.
   - Use **t-SNE** to visualize the data in two dimensions and inspect how the two target classes are distributed.

5. **Establish model comparisons**  
   Train and compare four classification algorithms:
   - Logistic Regression
   - k-Nearest Neighbors (k-NN)
   - Decision Tree
   - Random Forest

6. **Train, validate, and tune**  
   Split the data into **80% training and 20% testing**, using stratification for the target classes. Use **GridSearchCV** with 5-fold cross-validation to search selected hyperparameters for each classifier. The notebook also compares mean cross-validation accuracy.

7. **Evaluate and reflect**  
   Compare accuracy and classification reports, and visualize confusion matrices. Review the models' strengths and limitations, identify the most useful features discussed in the notebook, and note possible improvements for a future iteration.

---

## Libraries and Tools

The first project uses the following Python libraries:

| Library | How it is used |
| --- | --- |
| **pandas** | Load the CSV dataset, inspect and organize tabular data, and create result tables. |
| **NumPy** | Numerical computing support for the data science workflow. |
| **Matplotlib** | Create plots and visualizations. |
| **Seaborn** | Create statistical visualizations, including scatterplots and confusion-matrix heatmaps. |
| **scikit-learn** | Preprocess features, explore dimensionality reduction, train classifiers, tune hyperparameters, cross-validate, and evaluate model performance. |

### Key scikit-learn components

- **Preprocessing:** `OneHotEncoder`, `StandardScaler`
- **Dimensionality reduction and visualization:** `PCA`, `TSNE`
- **Model selection and validation:** `train_test_split`, `GridSearchCV`, `cross_val_score`
- **Classification models:** `LogisticRegression`, `KNeighborsClassifier`, `DecisionTreeClassifier`, `RandomForestClassifier`
- **Evaluation:** `accuracy_score`, `classification_report`, `confusion_matrix`

The notebook was developed in **Google Colab** using a Jupyter notebook (`.ipynb`) format. The saved code outputs and plots are included in the notebook for viewing on GitHub; GitHub displays these saved results but does not execute the notebook.

---

## Repository Contents

```text
.
├── README.md
├── DS218_Final_Requirement_GitHub.ipynb
└── personality.csv
```

As more projects are added, this index will grow. I may organize larger projects into their own folders with a notebook, supporting datasets, and project-specific notes.

---

## Run the First Project

### Option 1: Google Colab

1. Open [`DS218_Final_Requirement_GitHub.ipynb`](DS218_Final_Requirement_GitHub.ipynb) in Google Colab.
2. Upload `personality.csv` to the Colab session, or place it in the same working directory as the notebook.
3. Run the notebook cells in order, or select **Runtime → Run all**.

### Option 2: Run locally

1. Clone or download this repository.
2. Make sure `DS218_Final_Requirement_GitHub.ipynb` and `personality.csv` are in the same directory.
3. Install the libraries used by the notebook:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

4. Start Jupyter Notebook or JupyterLab and open the `.ipynb` file.
5. Run the cells from top to bottom.

---

## Scope and Limitations

This is an **exploratory academic exercise** using a small dataset of 100 records and a limited set of behavioral features. The notebook itself notes that the sample size, limited features, and possible self-identification bias constrain what can be concluded.

The model output should therefore be understood as predictions of the labels in this particular dataset—not as a reliable psychological assessment of a real person. The results are useful for practicing the machine learning workflow, comparing algorithms, and identifying questions for further investigation. They are not evidence that social-media behavior can definitively determine someone's personality.

Possible future improvements discussed in the notebook include collecting a larger dataset, adding behavioral features, and exploring more advanced approaches.

---

## About This Repository

I am building this repository as a public record of my progress from physics education toward data science and AI engineering. I expect the projects to be varied and imperfect; that is part of the process. Each mini-project is an opportunity to practice a new technique, strengthen my understanding, and make the next project better than the last.

Thanks for taking a look. Feedback and constructive suggestions are welcome.
