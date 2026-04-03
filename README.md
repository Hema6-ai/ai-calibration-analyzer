# 🔍 AI Confidence Calibration Analyzer

**Modeling AI Uncertainty using Markov Chains & Metropolis-Hastings**

---

## 🚀 Overview

Modern AI systems often produce **overconfident predictions**, where the reported confidence does not reflect true correctness.

This project provides an **interactive probabilistic simulation + real data analysis tool** to:

* Model AI behavior as a **Markov Chain**
* Apply **Metropolis-Hastings (MCMC)** sampling
* Analyze **stationary distributions**
* Evaluate **confidence calibration using real datasets**

---

## 🎯 Problem Statement

AI systems frequently fall into this critical failure mode:

> ⚠️ High confidence, but wrong predictions

We model AI predictions into 3 states:

| State | Meaning                    |
| ----- | -------------------------- |
| C1    | High Confidence & Correct  |
| C2    | High Confidence & Wrong ⚠️ |
| C3    | Low Confidence             |

---

## 🧠 Methodology

### 1. Markov Chain Modeling

* Define transition probabilities between states
* Simulate real-world prediction behavior

### 2. Metropolis-Hastings Algorithm

Used for sampling from target distribution:

α = min(1, π(x') / π(x))

* Accept / reject transitions
* Converges to stationary distribution

### 3. Stationary Distribution

* Empirical distribution from sampling
* Compared with target π

### 4. MAP Inference

* Detect most probable system state

---

## 📊 Key Features

### 🔁 Simulation Engine

* Step-by-step MH sampling
* Auto-run simulation
* Acceptance/rejection tracking

### 📈 Visualization

* Distribution comparison (π vs empirical)
* Confidence calibration curve
* Real-time updates

### 📂 Real Dataset Integration (🔥 Major Feature)

* Upload CSV dataset:

  ```
  prediction, confidence, actual
  ```
* Automatically:

  * Computes π from real data
  * Builds calibration curve from dataset
  * Detects overconfidence patterns

### 🎯 Calibration Analysis

* 5-bin confidence evaluation
* Detects:

  * Overconfidence
  * Underconfidence
  * Miscalibration

---

## 🌐 Live Demo

👉 https://hema6-ai.github.io/ai-calibration-analyzer/

---

## ⚙️ How It Works

### Step 1: Define States

* Configure prediction states (C1, C2, C3)
* Set target distribution π

### Step 2: Set Transition Matrix

* Each row must sum to 1
* Represents behavior transitions

### Step 3: (Optional) Upload Dataset

* Real data overrides synthetic assumptions
* π auto-updated from dataset

### Step 4: Run Simulation

* Observe:

  * Markov chain path
  * Acceptance decisions
  * Convergence behavior

### Step 5: Analyze Output

* Stationary distribution
* MAP state
* Calibration curve

---

## 📊 Example Insight

Even well-performing models may spend:

> ❗ Significant time in "High Confidence & Wrong" state

This indicates:

* Poor calibration
* Risk in real-world deployment

---

## 🛠️ Tech Stack

* HTML (UI structure)
* CSS (custom UI/UX)
* JavaScript (core logic)
* Chart.js (visualization)

---

## 🚧 Limitations

* Simplified 3-state model
* Dataset must follow strict format
* Calibration bins are fixed (5 bins)
* No deep model integration (yet)

---

## 🔮 Future Improvements

* Multi-class calibration support
* Advanced MCMC methods (HMC, Gibbs)
* Integration with real ML models (PyTorch / TensorFlow)
* Uncertainty metrics (ECE, Brier Score)
* Backend + API support

---

## 🧠 Key Insight

> Calibration is not about accuracy —
> it is about **trustworthiness of confidence**.

---

## 🏆 Use Cases

* 🏥 Medical AI validation
* 🤖 ML model calibration
* 📈 Financial prediction systems
* 🚗 Autonomous systems


