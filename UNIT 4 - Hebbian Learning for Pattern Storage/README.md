# Unit IV – Hebbian Learning for Pattern Storage

## 📌 Project Overview
This project demonstrates **Hebbian learning**, a biologically inspired neural learning rule. The goal is to store simple binary patterns in a network and **recall them correctly** using the learned weight matrix. Hebbian learning is based on the principle: "**Neurons that fire together, wire together**."

---

## 🎯 Objective
- Store multiple binary patterns in a network using Hebbian learning.  
- Recall stored patterns to verify memory retention.  
- Understand how correlation between neurons determines the weight matrix.  

---

## 🛠 Methodology
1. **Dataset**: Simple binary patterns (3×3 or 4×4 matrices) flattened into vectors.  
2. **Hebbian Learning Rule**:
   \[
   W = \sum_{p=1}^{P} x^{(p)} \cdot {x^{(p)}}^T
   \]
   - `x^(p)` → input pattern vector  
   - `P` → number of patterns  
   - Diagonal of `W` is set to 0 (no self-connections)  
3. **Recall Patterns**:
   \[
   y = \text{sign}(W \cdot x)
   \]
   - Output `y` should reproduce the original input pattern.  

---

## 📊 Results
- **Learned Weight Matrix**: Shows correlations between neurons.  
- **Recall**: All stored patterns are successfully recalled if the number of patterns is within network capacity.  
- **Observations**: Too many patterns can cause interference, reducing recall accuracy.  

---

## 📝 Key Takeaways
- Hebbian learning is a **simple, local learning rule** that forms the foundation of associative memory.  
- Effective for storing and recalling **binary patterns**.  
- Introduces concepts that are expanded in **Hopfield Networks** for robust associative memory.  

---

## 📌 Deliverables
1. Defined binary patterns  
2. Learned weight matrix (`W`)  
3. Recall demonstration  
4. Observations on pattern storage and retrieval  

