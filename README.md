# **🚀 SigmoidJump: Build Neural Networks from Scratch**  
*A beginner-friendly Python implementation of autograd and neural networks*  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![Neural Networks](https://img.shields.io/badge/Neural_Networks-From_Scratch-orange)  

## **✨ What is SigmoidJump?**  
SigmoidJump is a **lightweight neural network framework** built from scratch to help beginners understand:  
- How **backpropagation** really works  
- What happens inside **PyTorch/TensorFlow**  
- How to build **neurons, layers, and MLPs** with pure Python  

Perfect for students and aspiring ML engineers!  

---

## **🔧 Key Features**  
✅ **Autograd Engine** - Automatic differentiation like PyTorch  
✅ **Neural Network Components** - Neurons, Layers, and MLPs  
✅ **Activation Functions** - ReLU, Tanh, Sigmoid  
✅ **Training Loop** - Train models with gradient descent  
✅ **Visualization** - See computation graphs with Graphviz  

---

## **📦 Installation**  
```bash
pip install numpy matplotlib graphviz
```

---

## **🚀 Quick Start**  
### 1. **Create a Neuron**  
```python
from sigmoidjump import Value

# Inputs
x1 = Value(2.0, label='x1')  
x2 = Value(0.0, label='x2')  

# Weights  
w1 = Value(-3.0, label='w1')  
w2 = Value(1.0, label='w2')  

# Neuron computation  
n = x1*w1 + x2*w2 + Value(6.7, label='bias')  
out = n.tanh()  
out.backward()  # Magic happens here!
```

### 2. **Train a Neural Network**  
```python
model = MLP(3, [4, 4, 1])  # 3-layer network  

# Training loop  
for epoch in range(20):  
    loss = train_step(model, X, y)  
    print(f"Epoch {epoch}, Loss: {loss.data:.4f}")  
```

---

## **📊 Sample Output**  
```
Epoch 0, Loss: 5.1684  
Epoch 1, Loss: 2.8050  
...  
Epoch 19, Loss: 0.0648  # Loss decreasing! 🎉
```

---

## **📚 Learn Concepts**  
🔹 **How backpropagation works**  
🔹 **What gradients really are**  
🔹 **Building blocks of deep learning**  

---

## **📂 Project Files**  
- `sigmoidjump.ipynb` - Main implementation (Jupyter Notebook)  
- `README.md` - This guide  

---

## **💡 Why This Project?**  
- **No black boxes!** Understand every step of deep learning  
- **Perfect for resumes** - Shows core ML knowledge  
- **Fun to experiment with!**  

---

## **👨‍💻 Author**  
**Satyabrata Satapathy**  
📧 satya78550@gmail.com | 🔗 [GitHub](https://github.com/satya122id0889)  

---

**🌟 Star this repo if you find it useful!**  

--- 

This version keeps it **simple, engaging, and beginner-friendly** while highlighting the educational value. Adjust the links/emojis to your style! 🚀
