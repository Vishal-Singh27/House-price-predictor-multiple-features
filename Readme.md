# 🏠 House Price Predictor (Multiple Features)

This project predicts house prices using **Linear Regression** with multiple features derived from a single input—**house size**. It builds the model from scratch using custom cost and gradient descent functions, and visualizes the predictions to understand how well the model fits the data.

---

## 🔍 What the Project Does

- Takes a basic dataset of house sizes and prices  
- Creates polynomial features (e.g., size², size³, size⁴)  
- Applies feature scaling for better learning  
- Uses gradient descent to train the model  
- Predicts and visualizes house prices  

---

## 📊 Sample Data

| House Size (sq ft) | Price (in $1000s) |
|--------------------|-------------------|
| 10                 | 100               |
| 20                 | 200               |
| 30                 | 350               |
| 40                 | 600               |
| 70                 | 1000              |

---

## ⚙️ Feature Engineering

From the single input feature (House Size), the model creates the following additional features:

| Feature | Description              |
|---------|--------------------------|
| x       | House size               |
| x²      | House size squared       |
| x³      | House size cubed         |
| x⁴      | House size to the power 4|

This transforms the model into a **polynomial regression** model, allowing it to capture nonlinear relationships.

---

## 📐 Model Process

| Step                    | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| Feature Scaling         | All input features and outputs are standardized (mean = 0, std = 1)        |
| Cost Function           | Calculates how far off the predictions are (using Mean Squared Error)       |
| Gradient Descent        | Adjusts weights and bias to minimize the cost                              |
| Training Iterations     | Model is trained over thousands of updates for better accuracy              |

---

## 📈 Visualization

After training, the model's predictions are plotted against the original data:

- **Dots** show the actual house prices  
- **Line** shows the predicted prices by the model  

This helps us visually evaluate how well the model fits the data.

---

## 🧠 Key Learnings

- How to build a linear regression model from scratch  
- The role of polynomial features in modeling complex relationships  
- Why feature scaling matters  
- How gradient descent helps optimize model parameters  

---

## ✅ What's Next?

Ideas to improve this project:
- Add more input features (e.g., location, number of rooms)
- Use real-world datasets
- Introduce regularization to avoid overfitting
- Experiment with different learning rates or optimizers
