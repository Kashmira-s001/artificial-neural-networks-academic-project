# Unit III – Function Approximation using RBF Network

## 📌 Project Overview
This project demonstrates the use of a **Radial Basis Function (RBF) Network** to approximate the sine function. RBF networks are a type of neural network that use **radial basis functions as hidden neurons**, enabling them to approximate non-linear functions with high accuracy.

---

## 🎯 Objective
- Approximate the function `y = sin(x)` using an RBF network.  
- Visualize the **true function vs predicted approximation**.  
- Understand how **RBF centers and widths** affect function approximation.

---

## 🛠 Methodology
1. **Dataset**: Synthetic points sampled from `y = sin(x)`  
2. **RBF Network Architecture**:
   - Input layer: 1 neuron  
   - Hidden layer: 10 RBF neurons (Gaussian activation)  
   - Output layer: 1 linear neuron  
   - Training: Linear least squares for output weights  

3. **Steps**:
   - Initialize RBF centers and widths (σ)  
   - Compute hidden layer output using Gaussian RBF:  
     \[
     \phi_i(x) = \exp\Big(-\frac{||x - c_i||^2}{2\sigma_i^2}\Big)
     \]  
     where \(c_i\) is the center of neuron `i`.  
   - Solve for output weights using **pseudoinverse**: `W = pinv(Phi) @ y`  
   - Predict outputs: `y_pred = Phi @ W`  

---

## 📊 Results
- **True vs Predicted Curve**: RBF network closely follows the sine function.  
- **RBF Centers**: Marked along the input domain to show “local detectors”.  
- RBF network can **generalize non-linear functions** effectively.  

---

## 📝 Key Takeaways
- RBF networks are powerful for **function approximation** and regression tasks.  
- Centers and widths of RBF neurons determine **accuracy and smoothness** of approximation.  
- Linear output weights make training straightforward compared to MLP backpropagation.  

---

## 📌 Deliverables
1. Synthetic sine dataset  
2. RBF network implementation  
3. True vs predicted function plot  
4. Visualization of RBF centers  
5. Analysis of approximation accuracy  

