                                  AI Confidence Calibration Analyzer  
### Modeling AI Uncertainty using Markov Chains & Metropolis-Hastings  

---

## 🔍 Overview

Modern AI systems often produce **overconfident predictions**, where the confidence score does not match actual correctness.

This project models that behavior using:

- 🔗 Markov Chains  
- 🎯 Metropolis-Hastings (MCMC)  
- 📊 Stationary Distribution Analysis  
- 🏆 MAP Inference  

An interactive web tool is built to simulate and visualize this process.

---

## 🎯 Problem

AI models can exist in the following states:

- **C1:** High Confidence & Correct  
- **C2:** High Confidence & Wrong ⚠️  
- **C3:** Low Confidence  

### Goal:
- Model transitions between states  
- Estimate the true distribution using sampling  
- Identify the most probable state  

---

## 🧠 Methodology

### 1. Markov Chain  
A transition probability matrix defines how the system moves between states.

### 2. Metropolis-Hastings Algorithm  

\[
\alpha = \min \left(1, \frac{\pi(x')}{\pi(x)} \right)
\]

### 3. Simulation  
- Step-by-step sampling  
- Acceptance / rejection decisions  
- Convergence to stationary distribution  

---

## 💻 Features

- 🎨 Premium UI/UX interface  
- 📌 Editable state configuration  
- 🔢 Transition matrix validation  
- ⚙️ Real-time M-H simulation  
- ▶️ Step-by-step & auto-run modes  
- 📋 Iteration log (accept/reject tracking)  
- 📊 Stationary distribution visualization  
- 🏆 MAP inference detection  
- 💡 Insight generation  

---

## 🌐 Live Demo

👉 **[Open Tool](https://hema6-ai.github.io/ai-calibration-analyzer/)**  

---

## 🛠️ Tech Stack

- HTML  
- CSS (Custom UI Design)  
- JavaScript (Simulation Logic)  

---

## ⚙️ How It Works

1. Define states and probabilities (π)  
2. Set transition matrix (P)  
3. Validate constraints  
4. Run Metropolis-Hastings sampling  

### Observe:
- Markov chain path  
- Acceptance decisions  
- Converged distribution  

---

## 📊 Example Output

### Stationary Distribution
C1 ≈ 0.50
C2 ≈ 0.33
C3 ≈ 0.17


### MAP Inference

C1 (High Confidence & Correct)

---

## ⚠️ Key Insight

Even when AI performs well, it still spends time in:

> ❗ High Confidence & Wrong state  

This highlights the need for **better calibration techniques**.

---

## 📌 Use Cases

- 🏥 Medical AI  
- 🤖 ML Model Calibration  
- 📈 Financial Systems  
- 🚗 Autonomous Systems  

---

## 🚧 Limitations

- Simplified 3-state model  
- No real dataset integration  
- Approximate sampling  

---

## 🔮 Future Improvements

- Integrate real ML outputs  
- Scale to high-dimensional models  
- Use advanced MCMC methods  
- Add uncertainty metrics  

