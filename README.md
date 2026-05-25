# 🎯 Placement Prediction Model (Machine Learning Project)

This project is a simple **Machine Learning Classification Model** that predicts whether a student will get placed or not based on features like **CGPA** and **IQ**.

Built using **Python**, **Scikit-Learn**, **Pandas**, and **Matplotlib**.

---

## 🚀 Features

- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Selection
- Train-Test Split
- Feature Scaling using StandardScaler
- Logistic Regression Model
- Model Evaluation
- Decision Boundary Visualization
- Model Saving using Pickle

---

## 🛠️ Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- Mlxtend
- Pickle

---

## 📂 Project Structure

```bash
├── placement.csv            # Dataset
├── firstMLProjectCampusX.ipynb   # Jupyter Notebook
├── model.pkl                # Saved trained model
└── README.md
```

---

## 📊 Dataset Information

The dataset contains:

| Feature | Description |
|----------|-------------|
| CGPA | Student CGPA |
| IQ | Student IQ Score |
| Placement | Target Variable (Placed / Not Placed) |

---

## ⚙️ Machine Learning Workflow

### 1. Data Loading
Dataset loaded using Pandas.

```python
df = pd.read_csv('placement.csv')
```

### 2. Data Preprocessing

- Removed unnecessary columns
- Selected input & output features

### 3. Visualization

Scatter plots used for data understanding.

```python
plt.scatter(df['cgpa'], df['iq'], c=df['placement'])
```

### 4. Train-Test Split

```python
train_test_split(X, Y, test_size=0.1)
```

### 5. Feature Scaling

Used **StandardScaler**.

```python
scaler = StandardScaler()
```

### 6. Model Training

Implemented **Logistic Regression**.

```python
clf = LogisticRegression()
clf.fit(X_train, Y_train)
```

### 7. Model Evaluation

Accuracy Score:

```python
accuracy_score(Y_test, y_pred)
```

### 8. Model Deployment Preparation

Saved model using Pickle.

```python
pickle.dump(clf, open('model.pkl','wb'))
```

---

## 📈 Decision Boundary Visualization

Used `mlxtend.plotting` to visualize the model's decision regions.

```python
plot_decision_regions(X_train, Y_train.values, clf=clf)
```

---

## ▶️ How To Run

### Clone Repository

```bash
git clone https://github.com/yourusername/your-repo-name.git
```

### Install Dependencies

```bash
pip install numpy pandas matplotlib scikit-learn mlxtend
```

### Run Notebook

```bash
jupyter notebook
```

Open:

```bash
firstMLProjectCampusX.ipynb
```

---

## 🎓 Learning Outcomes

Through this project, I learned:

- Data preprocessing
- Feature scaling
- Logistic Regression
- Model evaluation
- Visualization techniques
- Saving ML models

---

## 📌 Future Improvements

- Add more features
- Hyperparameter tuning
- Web deployment using Flask/Streamlit
- Improve model accuracy

---

## 👨‍💻 Author

**Sudhanshu Baberwal**  
B.Tech Student | Machine Learning Enthusiast

GitHub: https://github.com/yourusername

---

⭐ If you like this project, consider giving it a **star**!