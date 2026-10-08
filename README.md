







<h1 align="center"> 💻 𝗠𝗟 𝗦𝗢𝗟𝗨𝗧𝗜𝗢𝗡𝗦</h1>



<br>





![BOOKS](https://raw.githubusercontent.com/Dreamerol/Dreamerol/992fd2d040b50ce71e58d732090cd255ec3f2270/COMP22.jpg)






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




# 🤖 Machine Learning From Scratch

### Understanding Machine Learning by building the algorithms myself.

Building ML algorithms from scratch to understand the **math, logic, and intuition** behind them — not just how to use a library.


---

## 🧠 About

<div align="left">

This repository contains my implementations and experiments with fundamental **Machine Learning algorithms**.

The main goal is to understand how Machine Learning works **under the hood** by implementing the core ideas and mathematics behind different algorithms.

</div>

<div align="left">

Instead of treating models as black boxes and simply using:

```python
model.fit(X, y)
model.predict(X_test)
```

I focus on understanding what happens behind the prediction — from **distances and probabilities** to **gradients, entropy, loss functions, and decision boundaries**.

</div>

---

## 📚 Algorithms

<table>
<tr>

<td width="50%" valign="top">

### 🔹 K-Nearest Neighbors

**Concepts**

* Euclidean distance
* Nearest neighbors
* Majority voting
* Classification

```python
def euclidean_distance(a, b):
    return np.sqrt(
        sum((a[i] - b[i]) ** 2
            for i in range(len(a)))
    )
```

```python
k_nearest = np.argsort(distances)[:k]
labels = y_train[k_nearest]

prediction = Counter(
    labels
).most_common(1)[0][0]
```

</td>

<td width="50%" valign="top">

### 🌳 Decision Tree

**Concepts**

* Entropy
* Information Gain
* Recursive splitting
* Decision nodes
* Leaf nodes

```python
information_gain = (
    entropy(parent)
    - left_weight * entropy(left)
    - right_weight * entropy(right)
)
```

```python
if feature_value <= threshold:
    go_left()
else:
    go_right()
```

</td>

</tr>

<tr>

<td width="50%" valign="top">

### 📈 Logistic Regression

**Concepts**

* Sigmoid function
* Binary classification
* Cross-entropy loss
* Gradient descent

```python
def sigmoid(z):
    return 1 / (1 + np.exp(-z))
```

```python
prediction = 1 if probability >= 0.5 else 0
```

The model learns parameters by minimizing the **cost function** using gradient descent.

</td>

<td width="50%" valign="top">

### 🎲 Naive Bayes

**Concepts**

* Prior probability
* Likelihood
* Posterior probability
* Gaussian distribution

```python
posterior = (
    likelihood * prior
)
```

```python
prediction = classes[
    np.argmax(posteriors)
]
```

The implementation uses **Gaussian likelihoods** for continuous features.

</td>

</tr>

<tr>

<td width="50%" valign="top">

### 📊 Linear Regression

**Concepts**

* Simple regression
* Multiple regression
* Coefficients
* Intercept
* Prediction
* R² score

```python
model = LinearRegression()

model.fit(X, y)

predictions = model.predict(X)
```

The goal is to find a line that best represents the relationship between the input features and the target.

</td>

<td width="50%" valign="top">

### 🧮 Polynomial Regression

**Concepts**

* Polynomial features
* Non-linear relationships
* Feature transformation
* Degree

```python
poly = PolynomialFeatures(
    degree=2
)

X_poly = poly.fit_transform(X)
```

```python
model = LinearRegression()
model.fit(X_poly, y)
```

Polynomial regression allows linear regression to model **non-linear patterns**.

</td>

</tr>

<tr>

<td width="50%" valign="top">

### ⚡ Support Vector Machine

**Concepts**

* Maximum margin
* Support vectors
* Hinge loss
* L2 regularization
* Gradient descent

```python
condition = (
    y * np.dot(x, w) - b >= 1
)
```

The objective is to find a decision boundary with the **largest possible margin** between classes.

</td>

<td width="50%" valign="top">

### 🔄 Machine Learning Workflow

Most implementations follow the same basic pipeline:

```text
Dataset
   ↓
Features & Target
   ↓
Train / Test Split
   ↓
Training
   ↓
Prediction
   ↓
Evaluation
```

This project focuses on understanding every step of this process.

</td>

</tr>
</table>

---

## 🎯 Classification vs Regression

| Type              | Goal                       | Algorithms                                                |
| ----------------- | -------------------------- | --------------------------------------------------------- |
| 🟢 Classification | Predict a class            | KNN, Decision Tree, Logistic Regression, Naive Bayes, SVM |
| 🔵 Regression     | Predict a continuous value | Linear Regression, Polynomial Regression                  |

---

## 🧩 Core Concepts

| Concept                   | Purpose                               |
| ------------------------- | ------------------------------------- |
| 📏 Euclidean Distance     | Measures distance between data points |
| 🌳 Entropy                | Measures impurity in a dataset        |
| 📈 Information Gain       | Determines the best tree split        |
| 🔢 Sigmoid                | Converts values into probabilities    |
| 🎲 Bayes Theorem          | Calculates posterior probabilities    |
| 📉 Gradient Descent       | Optimizes model parameters            |
| ⚖️ Regularization         | Helps reduce overfitting              |
| 📐 Margin                 | Determines the SVM decision boundary  |
| 🔄 Feature Transformation | Creates polynomial features           |

---

## 🛠️ Tech Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge\&logo=numpy\&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge\&logo=pandas\&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge\&logo=scikit-learn\&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge\&logo=plotly\&logoColor=white)

</div>

---

## 📁 Project Structure

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

## 🚀 Why This Project?

Machine Learning becomes much easier to understand when you stop treating algorithms as black boxes.

This project is about learning **how and why** the algorithms work.

```text
Understand the Math
        ↓
Understand the Algorithm
        ↓
Implement It
        ↓
Test It
        ↓
Understand the Model
```

---

## 🔮 Future Improvements

* [ ] Add model evaluation metrics
* [ ] Add confusion matrices
* [ ] Visualize decision boundaries
* [ ] Add more algorithms
* [ ] Improve implementations and documentation
* [ ] Compare from-scratch implementations with Scikit-learn
* [ ] Add mathematical explanations
* [ ] Add datasets and experiments

---

<div align="center">

### 🧠 Don't just use Machine Learning. Understand it.

**Learn the math. Build the algorithm. Understand the model.**


<br><br>




</div>

</div>

</div>




---






<br><br><br>






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












