# Fruits_Classification-using-Machine-Learning
<div align="center">

# 🍎 Fruit Classification Using Machine Learning

### Supervised Learning • Decision Tree Classification

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge\&logo=python\&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-orange?style=for-the-badge)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Supervised-green?style=for-the-badge)
![Decision Tree](https://img.shields.io/badge/Algorithm-Decision%20Tree-success?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-Project-black?style=for-the-badge\&logo=github)

</div>

---

# 📖 Overview

This project is a beginner-friendly **Machine Learning fruit classification system** developed using Python and Scikit-learn.

The project uses a **Decision Tree Classifier** to classify fruits based on three features:

* ⚖️ Weight
* 🎨 Color
* ✋ Texture

The model is trained using labeled examples of four fruits:

* 🍎 Apple
* 🍊 Orange
* 🍌 Banana
* 🥭 Mango

The first three fruits are required by the assignment, while **Mango was added as the optional challenge**.

The purpose of this project is to understand the basic Machine Learning workflow:

**Features → Labels → Training → Model → Prediction**

---

# 🎯 Objectives

The main objectives of this project are to:

* Understand basic Machine Learning concepts.
* Understand **Supervised Learning**.
* Create a small fruit dataset.
* Identify features and labels.
* Train a Decision Tree Classifier.
* Use `model.fit()` to train the model.
* Use `model.predict()` to classify new fruits.
* Test the model using new feature values.
* Understand how a Decision Tree learns classification patterns.
* Practice using Scikit-learn in Python.

---

# 🧠 Machine Learning Concepts

## 1. Features

Features are the input information given to the Machine Learning model.

This project uses three features:

| Feature | Description                               |
| ------- | ----------------------------------------- |
| Weight  | Weight of the fruit in grams              |
| Color   | Numerical representation of fruit color   |
| Texture | Numerical representation of fruit texture |

### Color Encoding

```text
1 = Red
2 = Orange
3 = Yellow
4 = Green
```

### Texture Encoding

```text
1 = Smooth
2 = Rough
```

---

## 2. Labels

Labels are the correct answers associated with the training examples.

The labels used in this project are:

```text
Apple
Orange
Banana
Mango
```

---

## 3. Supervised Learning

This project uses **Supervised Learning** because the model is trained using examples where the correct fruit labels are already known.

For example:

```text
[150, 1, 1] → Apple
[180, 2, 1] → Orange
[120, 3, 2] → Banana
[200, 4, 1] → Mango
```

The model learns patterns from these examples.

---

# 🌳 Decision Tree Classifier

A Decision Tree is a Machine Learning algorithm used for classification.

The model learns decision rules from the training data and uses those rules to classify new examples.

In this project, the Decision Tree learns from:

```text
Weight + Color + Texture
```

and predicts:

```text
Apple / Orange / Banana / Mango
```

The rules are **learned by the model** rather than manually written using `if-else` statements.

---

# 📊 Dataset

The project contains **16 training examples**.

### Training examples

| Fruit  | Weight | Color | Texture |
| ------ | -----: | ----: | ------: |
| Apple  |    150 |     1 |       1 |
| Apple  |    160 |     1 |       1 |
| Apple  |    140 |     1 |       2 |
| Apple  |    170 |     1 |       1 |
| Orange |    180 |     2 |       1 |
| Orange |    190 |     2 |       1 |
| Orange |    170 |     2 |       2 |
| Orange |    200 |     2 |       1 |
| Banana |    120 |     3 |       2 |
| Banana |    110 |     3 |       2 |
| Banana |    130 |     3 |       1 |
| Banana |    125 |     3 |       2 |
| Mango  |    200 |     4 |       1 |
| Mango  |    220 |     4 |       1 |
| Mango  |    180 |     4 |       1 |
| Mango  |    210 |     4 |       2 |

---

# 🔢 Training Process

The model is trained using:

```python
model.fit(features, labels)
```

The `fit()` function allows the Decision Tree to learn patterns from the training examples.

The basic workflow is:

```text
Training Features
       +
Training Labels
       ↓
 model.fit()
       ↓
Trained Decision Tree
```

---

# 🔮 Prediction

After training, new fruit examples are given to the model.

For example:

```python
new_fruit_1 = [155, 1, 1]
new_fruit_2 = [185, 2, 1]
new_fruit_3 = [115, 3, 2]
new_fruit_4 = [205, 4, 1]
```

The model predicts the fruit using:

```python
model.predict()
```

Expected predictions:

```text
Fruit 1 → Apple
Fruit 2 → Orange
Fruit 3 → Banana
Fruit 4 → Mango
```

---

# 🥭 Optional Challenge

The original project requires:

* Apple
* Orange
* Banana

As an optional challenge, a fourth fruit can be added.

For this project, **Mango** was added.

Mango training examples:

```text
[200, 4, 1]
[220, 4, 1]
[180, 4, 1]
[210, 4, 2]
```

A new Mango example is also tested:

```text
[205, 4, 1]
```

This allows the model to classify four different fruit categories.

---

# 📂 Project Structure

```text
Fruit_Classification_ML/
│
├── fruit_classification.py
│
├── README.md
│
└── screenshot/
    └── program_output.png
```

---

# 🛠️ Technologies Used

| Technology    | Purpose                  |
| ------------- | ------------------------ |
| Python        | Programming language     |
| Scikit-learn  | Machine Learning library |
| Decision Tree | Classification algorithm |
| VS Code       | Code editor              |
| GitHub        | Project hosting          |

---

# 📦 Installation

First, make sure Python is installed.

Then install Scikit-learn:

```bash
pip install scikit-learn
```

---

# 🚀 How to Run the Project

### Step 1

Clone or download this GitHub repository.

### Step 2

Open the project in VS Code or another Python editor.

### Step 3

Open:

```text
fruit_classification.py
```

### Step 4

Run the program:

```bash
python fruit_classification.py
```

### Step 5

View the predictions in the terminal.

---

# 🖥️ Example Output

```text
==========================================
       FRUIT CLASSIFICATION SYSTEM
==========================================

New Fruit 1: [155, 1, 1]
Prediction : apple

New Fruit 2: [185, 2, 1]
Prediction : orange

New Fruit 3: [115, 3, 2]
Prediction : banana

New Fruit 4: [205, 4, 1]
Prediction : mango

==========================================
          ADDITIONAL TESTING
==========================================

Test Fruit 1 : [145, 1, 1] -> apple
Test Fruit 2 : [195, 2, 1] -> orange
Test Fruit 3 : [118, 3, 2] -> banana
Test Fruit 4 : [215, 4, 1] -> mango

==========================================
          FINAL PREDICTIONS
==========================================

Fruit 1 prediction: apple
Fruit 2 prediction: orange
Fruit 3 prediction: banana
Fruit 4 prediction: mango

Model testing completed successfully!
==========================================
```

---

# 📚 Important Functions

### `DecisionTreeClassifier()`

Creates the Decision Tree Machine Learning model.

```python
model = DecisionTreeClassifier()
```

### `model.fit()`

Trains the model using features and labels.

```python
model.fit(features, labels)
```

### `model.predict()`

Predicts the class of new fruit examples.

```python
model.predict(new_fruit)
```

---

# 📝 Project Requirements Completed

* [x] Scikit-learn imported
* [x] DecisionTreeClassifier used
* [x] 16 training examples created
* [x] Apple included
* [x] Orange included
* [x] Banana included
* [x] Mango added as optional challenge
* [x] Weight used as a feature
* [x] Color used as a feature
* [x] Texture used as a feature
* [x] Labels created
* [x] Model trained using `.fit()`
* [x] At least 3 new fruits tested
* [x] Predictions printed
* [x] Additional feature values tested
* [x] Code commented and understandable

---

# 🎓 Learning Outcomes

After completing this project, I learned:

* What Machine Learning is.
* What Supervised Learning means.
* What features and labels are.
* How to create a small Machine Learning dataset.
* How to train a Decision Tree Classifier.
* How `model.fit()` works.
* How `model.predict()` works.
* How a model can classify new data.
* How to use Scikit-learn.
* How to organize and upload a Machine Learning project to GitHub.

---

# 👨‍🎓 Student Information

**Name:** Ali Raza

**Roll Number:** 1006

**Section:** 2026

**Course:** AI, Machine Learning and Deep Learning

**Project:** Fruit Classification Using Machine Learning

---

<div align="center">

### 🍎 🍊 🍌 🥭

**Fruit Classification using Machine Learning**

**Made with Python & Scikit-learn**

</div>
