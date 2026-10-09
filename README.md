







<h1 align="center">💻 𝗔𝗜 𝗦𝗧𝗨𝗗𝗜𝗢 → 𝗔𝗜 & 𝗠𝗟 𝗦𝗢𝗟𝗨𝗧𝗜𝗢𝗡𝗦</h1>   




<br>




<div align="center">

<a href="https://github.com/Dreamerol/AI-STUDIO">
  <img 
    src="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/MIHAELA%20KOSEVA-AI-STUDIO.png"
    width="100%"
    alt="Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineering, AI Engineer, Applied Machine Learning, Data Science, Software Engineer, Backend Engineer, REST APIs, Python, C++, Java, SQL, Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Sofia "
  />
</a>

</div>






<br>

<br>

<br>










<div align="center">

<a href="https://github.com/Dreamerol/CARDFOLIO">

<img
src="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/TECH-STACK-mihaela-koseva.png"
width="100%"
alt="Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineering, AI Engineer, Applied Machine Learning, Data Science, Software Engineer, Backend Engineer, REST APIs, Python, C++, Java, SQL, Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineer, Sofia, Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Sofia"
/>

</a>

</div>










<br>

















<div align="center">



<table>
<tr>

<td align="center" width="12%">
<span style="font-size:1.55em;">🌐</span><br>
<span style="font-size:1.4em;"><a href="https://dreamerol.github.io/MIHAELA-KOSEVA-AI/">𝗪𝗘𝗕𝗦𝗜𝗧𝗘</a></span>
</td>


<td align="center"><span style="font-size:1.3em;">│</span></td>

<td align="center" width="12%">
<span style="font-size:1.55em;">⚛️</span><br>
<span style="font-size:1.4em;"><a href="https://github.com/Dreamerol/AI-STUDIO">𝗔𝗜𝗦𝗧𝗨𝗗𝗜𝗢</a></span>
</td>


<td align="center"><span style="font-size:1.3em;">│</span></td>

<td align="center" width="12%">
<span style="font-size:1.55em;">🟢</span><br>
<span style="font-size:1.4em;"><a href="https://github.com/Dreamerol/PORTFOLIO">𝗣𝗢𝗥𝗧𝗙𝗢𝗟𝗜𝗢</a></span>
</td>

<td align="center"><span style="font-size:1.3em;">│</span></td>

<td align="center" width="12%">
<span style="font-size:1.55em;">🧩</span><br>
<span style="font-size:1.4em;"><a href="https://github.com/Dreamerol/CARDFOLIO">𝗥𝗘𝗣𝗢𝗦</a></span>
</td>

<td align="center"><span style="font-size:1.3em;">│</span></td>

<td align="center" width="12%">
<span style="font-size:1.55em;">📊</span><br>
<span style="font-size:1.4em;"><a href="https://github.com/Dreamerol/ALLSTATS">𝗦𝗧𝗔𝗧𝗦</a></span>
</td>

<td align="center"><span style="font-size:1.3em;">│</span></td>

<td align="center" width="12%">
<span style="font-size:1.55em;">✅</span><br>
<span style="font-size:1.4em;"><a href="https://github.com/Dreamerol/RESUME">𝗥𝗘𝗦𝗨𝗠𝗘</a></span>
</td>

<td align="center"><span style="font-size:1.3em;">│</span></td>

<td align="center" width="12%">
<span style="font-size:1.55em;">🔗</span><br>
<span style="font-size:1.4em;"><a href="https://www.linkedin.com/in/mihaela-koseva-software-engineer">𝗟𝗜𝗡𝗞𝗘𝗗𝗜𝗡</a></span>
</td>

<td align="center"><span style="font-size:1.3em;">│</span></td>

<td align="center" width="12%">
<span style="font-size:1.55em;">✉️</span><br>
<span style="font-size:1.4em;"><a href="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/MIHAELA_KOSEVA_VIZITKA.jpg">𝗖𝗢𝗡𝗧𝗔𝗖𝗧</a></span>
</td>

</tr>
</table>

</div>


























---







<div align="left">

<div align="left">





<br><br>





# 🤖 Machine Learning Algorithms From Scratch

### 🧠 Learning ML by Building It


A collection of Machine Learning algorithms implemented from scratch in Python.

<br>

**KNN • Decision Trees • Logistic Regression • Naive Bayes • Linear Regression • Polynomial Regression • Support Vector Machines (SVM)**



---

## 📚 Algorithms

<table>
<tr>

<td width="50%" valign="top">

## 🔵 K-Nearest Neighbors

KNN classifies a new point based on the classes of its closest neighbors.

### Main idea

```text
New Point
    ↓
Calculate distances
    ↓
Find K nearest points
    ↓
Majority Voting
    ↓
Predicted Class
```

### Core implementation

```python
def euclidean_distance(a, b):
    return np.sqrt(
        sum([(a[i] - b[i])**2 for i in range(len(a))])
    )
```

```python
class KNN:
    def __init__(self, k):
        self.k = k

    def fit(self, X, y):
        self.X_train = X
        self.y_train = y

    def predict_class(self, new_point):
        distances = [
            euclidean_distance(point, new_point)
            for point in self.X_train
        ]

        k_nearest_indices = np.argsort(distances)[:self.k]

        k_nearest_labels = [
            self.y_train[i]
            for i in k_nearest_indices
        ]

        return Counter(
            k_nearest_labels
        ).most_common(1)[0][0]
```

**Concepts:** Euclidean Distance • Nearest Neighbors • Majority Voting

</td>

<td width="50%" valign="top">

## 🌳 Decision Tree

The Decision Tree recursively splits the dataset using the feature and threshold that provide the highest information gain.

### Main idea

```text
             Root
              │
        Best Feature?
          /       \
       Left       Right
       /             \
    Split            Split
     / \              / \
   Leaf Leaf        Leaf Leaf
```

### Information Gain

```python
def information_gain(self, parent_y, left_y, right_y):

    left_weight = len(left_y) / len(parent_y)
    right_weight = len(right_y) / len(parent_y)

    return self.entropy(parent_y) - (
        left_weight * self.entropy(left_y)
        + right_weight * self.entropy(right_y)
    )
```

### Entropy

```python
def entropy(self, y):
    entropy = 0

    class_labels = np.unique(y)

    for class_label in class_labels:
        p = len(y[y == class_label]) / len(y)
        entropy -= p * np.log2(p)

    return entropy
```

**Concepts:** Entropy • Information Gain • Recursive Splitting • Leaf Nodes

</td>

</tr>

<tr>

<td width="50%" valign="top">

## 📈 Logistic Regression

Logistic Regression predicts the probability of belonging to a class using the sigmoid function.

### Sigmoid

```python
def sigmoid(z):
    return 1 / (1 + np.exp(-z))
```

### Prediction

```python
def predict(X, w, b):

    preds = np.zeros(len(X))

    for i in range(len(X)):

        z = np.dot(w, X[i]) + b
        g = sigmoid(z)

        preds[i] = 1 if g >= 0.5 else 0

    return preds
```

### Gradient Descent

```python
w -= alpha * grad_w
b -= alpha * grad_b
```

The model minimizes the **Binary Cross-Entropy Loss**.

**Concepts:** Sigmoid • Cross-Entropy • Gradients • Gradient Descent

</td>

<td width="50%" valign="top">

## 🎲 Naive Bayes

Naive Bayes predicts the class with the highest posterior probability.

### Main idea

```text
Prior Probability
       ×
Likelihood
       ↓
Posterior Probability
       ↓
Most Probable Class
```

### Gaussian Likelihood

```python
likelihood *= (
    1 / (np.sqrt(2 * np.pi) * std)
) * np.exp(
    -((row[feature] - mean)**2)
    / (2 * std**2)
)
```

### Prediction

```python
posteriors = []

for i in range(len(self.classes)):

    likelihood = self.compute_likelihood(
        row, i
    )

    posteriors.append(
        likelihood * self.priors[i]
    )

prediction = self.classes[
    np.argmax(posteriors)
]
```

**Concepts:** Bayes' Theorem • Prior • Likelihood • Posterior • Gaussian Distribution

</td>

</tr>

<tr>

<td width="50%" valign="top">

## 📏 Linear Regression

Linear Regression models the relationship between input variables and a continuous target.

### Simple Linear Regression

```text
y = ax + b
```

### Multiple Linear Regression

```text
y = a₁x₁ + a₂x₂ + ... + b
```

### Implementation

```python
model = LinearRegression()

model.fit(
    x.reshape(-1, 1),
    y
)

print(model.coef_)
print(model.intercept_)
```

### Prediction

```python
y_pred = model.predict(
    x.reshape(-1, 1)
)
```

### Evaluation

```python
model.score(
    x.reshape(-1, 1),
    y
)
```

The score represents the **R² coefficient of determination**.

</td>

<td width="50%" valign="top">

## 🧮 Polynomial Regression

Polynomial Regression allows a linear model to represent non-linear relationships.

### Degree 2

```text
[1, x, x²]
```

### Implementation

```python
poly = PolynomialFeatures(
    degree=2
)

X_poly = poly.fit_transform(X)

lin = LinearRegression()

lin.fit(
    X_poly,
    y
)
```

For multiple variables, polynomial features can also include interactions:

```text
x₁²
x₂²
x₁x₂
```

This allows the model to represent curved relationships between variables.

**Concepts:** Polynomial Features • Non-Linear Relationships • Feature Transformation

</td>

</tr>

<tr>

<td width="50%" valign="top">

## ⚔️ Support Vector Machine

SVM searches for a decision boundary with the **maximum margin** between classes.

### Main idea

```text
Class -1              Class +1

 ● ● ●                 ▲ ▲ ▲
 ● ● ●                 ▲ ▲ ▲
      \               /
       \    Margin   /
        \           /
         \         /
          ─────────
         Decision
         Boundary
```

### Labels

```python
y_ = np.where(
    y <= 0,
    -1,
    1
)
```

### Margin Condition

```python
condition = (
    y_[idx]
    * (np.dot(x_i, self.W) - self.bias)
    >= 1
)
```

If the point is correctly classified and outside the margin, only the regularization term is updated.

Otherwise, the hinge-loss gradient is applied.

**Concepts:** Maximum Margin • Hinge Loss • Regularization • Gradient Descent

</td>

<td width="50%" valign="top">

## 🔄 Common ML Workflow

All algorithms follow a similar general workflow:

```text
          Dataset
             ↓
      Split X and y
             ↓
      Train / Test Split
             ↓
        Train Model
             ↓
         Predict
             ↓
       Evaluate
```

### Train / Test Split

```python
X_train, X_test, \
y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.2
)
```

### Accuracy

For classification models:

```python
accuracy = np.mean(
    predictions == y_test
) * 100

print(accuracy)
```

This project focuses on understanding what happens **inside** the models instead of simply calling:

```python
model.fit(X, y)
model.predict(X_test)
```

</td>

</tr>
</table>

---

# 🧠 Concepts Covered

<div align="left">

| 📐 Mathematics     | 🤖 Machine Learning   | 🛠️ Tools    |
| ------------------ | --------------------- | ------------ |
| Euclidean Distance | KNN                   | NumPy        |
| Entropy            | Decision Tree         | Pandas       |
| Information Gain   | Naive Bayes           | Matplotlib   |
| Probability        | Logistic Regression   | Scikit-learn |
| Derivatives        | SVM                   | Python       |
| Gradient Descent   | Linear Regression     |              |
| Regularization     | Polynomial Regression |              |

</div>

---

# ⚖️ Classification vs Regression

```text
                 Machine Learning
                       │
             ┌─────────┴─────────┐
             │                   │
      Classification         Regression
             │                   │
      ┌──────┼──────┐       ┌────┴────┐
      │      │      │       │         │
     KNN    Tree   SVM    Linear   Polynomial
      │      │      │     Regression Regression
      │      │      │
 Logistic  Naive
 Regression Bayes
```

---

# 🛠️ Technologies

```text
Python
 ├── NumPy
 ├── Pandas
 ├── Matplotlib
 └── Scikit-learn
```

---

# 📂 Project Structure

```text
machine-learning/
│
├── data/
│   └── data.csv
│
├── knn.py
├── decision_tree.py
├── logistic_regression.py
├── naive_bayes.py
├── linear_regression.py
├── polynomial_regression.py
├── svm.py
│
└── README.md
```

---

# 🎯 Project Goal

The goal is simple:

> **Don't just use Machine Learning. Understand it.**

Instead of treating ML algorithms as black boxes, this project breaks them down into their fundamental mathematical and algorithmic components.

From calculating the distance between two points...

```text
KNN
 ↓
Distance
```

to finding the best split...

```text
Decision Tree
 ↓
Entropy
 ↓
Information Gain
```

to optimizing weights...

```text
Logistic Regression
 ↓
Gradient
 ↓
Gradient Descent
```

and maximizing the margin...

```text
SVM
 ↓
Hinge Loss
 ↓
Maximum Margin
```

the goal is to understand **why the algorithms work**, not only how to call them.

---

# 🚀 Future Improvements

* [ ] Feature Scaling
* [ ] Confusion Matrix
* [ ] Precision / Recall / F1 Score
* [ ] Cross-Validation
* [ ] Hyperparameter Tuning
* [ ] Better Visualizations
* [ ] Compare From-Scratch vs Scikit-learn
* [ ] More Datasets
* [ ] Model Performance Comparison
* [ ] More Machine Learning Algorithms


<br>


---


<div align="center">


### ⭐ Built to learn. Built to understand. Built from scratch.

**Machine Learning — one algorithm at a time. **

</div>




</div>

</div>






---






<br>






<h2 align="center">⭐ Explore repos & star what you find interesting</h2>













<div align="center">

<p style="font-size:10px; line-height:1.6; letter-spacing:0.2px;">

Mihaela Koseva (Михаела Косева) • Sofia University (Софийски университет) • AI Engineer • Software Engineer • Backend Engineer • Data Systems & APIs • Applied Machine Learning • Deep Learning • Neural Networks • Model Training • Data Pipelines • Data Science • LLMs • Python • C++ • Java • Clojure • SQL • PyTorch • TensorFlow • Scikit-learn • Pandas • NumPy • ETL • Data Modeling • MLOps
</p>

<p style="font-size:10px; opacity:0.7;">
© 2026 Mihaela Koseva (Михаела Косева) • Софийски университет • Original portfolio design.
</p>

<p style="font-size:10px; opacity:0.7;">
🔗 Explore on GitHub:
<a href="https://github.com/Dreamerol">Mihaela Koseva (Михаела Косева) • Software Engineer • AI • ML • Dreamerol</a>
</p>

</div>





















<br><br><br>









<div align="center">

<a href="https://github.com/Dreamerol/CARDFOLIO">
  <img 
    src="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/MIHAELA%20KOSEVA-DREAMEROL.png"
    width="100%"
    alt="Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineering, AI Engineer, Applied Machine Learning, Data Science, Software Engineer, Backend Engineer, REST APIs, Python, C++, Java, SQL"
  />
</a>

</div>












<br><br><br>








---








<table align="center" cellspacing="0" cellpadding="2">
<tr>

<td>
<a href="https://www.linkedin.com/in/mihaela-koseva-software-engineer" target="_blank">
<img src="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/Butoni%20LINKEDIN.png" height="130"
alt="Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineering, AI Engineer, Applied Machine Learning, Data Science, Software Engineer, Backend Engineer, REST APIs, Python, C++, Java, SQL">
</a>
</td>


<td>
<a href="https://github.com/Dreamerol" target="_blank">
<img src="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/Butoni%20GITHUB.png" height="130"
alt="Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineering, AI Engineer, Applied Machine Learning, Data Science, Software Engineer, Backend Engineer, REST APIs, Python, C++, Java, SQL">
</a>
</td>


<td>
<a href="https://github.com/Dreamerol/CARDFOLIO" target="_blank">
<img src="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/Butoni%20REPOSITORIES.png" height="130"
alt="Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineering, AI Engineer, Applied Machine Learning, Data Science, Software Engineer, Backend Engineer, REST APIs, Python, C++, Java, SQL">
</a>
</td>


<td>
<a href="https://github.com/Dreamerol/ALLSTATS" target="_blank">
<img src="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/Butoni%20STATS.png" height="130"
alt="Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineering, AI Engineer, Applied Machine Learning, Data Science, Software Engineer, Backend Engineer, REST APIs, Python, C++, Java, SQL">
</a>
</td>


<td>
<a href="https://github.com/Dreamerol/RESUME" target="_blank">
<img src="https://raw.githubusercontent.com/Dreamerol/Dreamerol/main/Butoni%20RESUME.png" height="130"
alt="Mihaela Koseva (Михаела Косева), Sofia University (Софийски университет), Software Engineering, AI Engineer, Applied Machine Learning, Data Science, Software Engineer, Backend Engineer, REST APIs, Python, C++, Java, SQL">
</a>
</td>

</tr>
</table>





<br><br><br>










