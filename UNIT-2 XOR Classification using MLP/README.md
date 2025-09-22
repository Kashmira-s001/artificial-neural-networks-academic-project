# Unit II – XOR Classification using MLP

## 📌 Project Overview
This project demonstrates the use of a **Multilayer Perceptron (MLP)** to classify the XOR logic function. XOR is a **classic non-linearly separable problem**, which cannot be solved by a simple perceptron. The MLP uses a **hidden layer with sigmoid activation** and backpropagation to learn the XOR mapping.

---

## 🎯 Objective
- Train an MLP to classify XOR inputs correctly.
- Visualize the **learning curve** and **decision boundary**.
- Compare MLP performance with a simple perceptron.

---

## 🛠 Methodology
1. **Dataset**: XOR truth table  
   | Input 1 | Input 2 | XOR Output |
   |---------|---------|------------|
   | 0       | 0       | 0          |
   | 0       | 1       | 1          |
   | 1       | 0       | 1          |
   | 1       | 1       | 0          |

2. **MLP Architecture**:
   - Input layer: 2 neurons  
   - Hidden layer: 2 neurons (sigmoid activation)  
   - Output layer: 1 neuron (sigmoid activation)  
   - Loss: Mean Squared Error (MSE)  
   - Optimizer: Gradient Descent  

3. **Training**:
   - Forward propagation → compute output  
   - Compute loss  
   - Backpropagation → update weights and biases  
   - Repeat for 10,000 epochs  

---

## 📊 Results
- **Accuracy**: 100% on XOR dataset  
- **Learning Curve**: Shows MSE decreasing steadily  
- **Decision Boundary**: MLP successfully separates XOR classes, unlike a single-layer perceptron  

### Comparison to Perceptron

| Feature             | Perceptron       | MLP                  |
|--------------------|----------------|--------------------|
| Linear Separation  | ✅ Only linear  | ❌ Linear & Non-linear |
| Hidden Layers      | ❌ None         | ✅ One or more       |
| XOR Classification | ❌ Fails        | ✅ Succeeds          |
| Complexity         | Low             | Moderate             |

---

## 📝 Key Takeaways
- MLPs can solve **non-linearly separable problems**.  
- Hidden layers enable **non-linear transformations** and complex decision boundaries.  
- This project illustrates the **power of backpropagation** in training neural networks.  

---

## 📌 Deliverables
1. XOR dataset table  
2. MLP training code with backpropagation  
3. Learning curve plot  
4. Decision boundary plot  
5. Accuracy metric  

