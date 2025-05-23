# Simulated-Cognitive-Effects-of-Magnesium-L-Threonate

# 🧠 Simulating the Cognitive Effects of Magnesium L-Threonate

This project uses a biologically inspired simulation to explore how Magnesium L-Threonate (MgT) might enhance memory through brain-level mechanisms — and leverages AI to predict cognitive outcomes.

---

## 📌 Project Overview

- Simulates a simplified but science-informed pathway:
  **MgT → ↑ Brain Mg²⁺ → ↑ NR2B → ↑ LTP → ↑ Synaptic Density → ↑ Memory**
- Incorporates additional biological factors like **Estrogen** and **BDNF** to reflect realistic variability in NR2B regulation.
- Trains a **Multi-Layer Perceptron Regressor (MLP)** to learn how upstream features influence memory performance.
- Analyzes feature importance to identify what the AI sees as the most influential predictors of cognition.

---

## 📊 Dataset Details

This dataset was synthetically generated using GPT-4 with guidance from published neuroscience research (e.g., *Liu et al., Neuron, 2010*). It is not based on real patient data.

Each simulated subject includes:
- `Group`: Supplement type (Control, Citrate, Threonate)
- `Brain_Mg`: Estimated brain magnesium level
- `Estrogen`: Simulated hormonal influence
- `BDNF`: Neurotrophic factor level
- `Age`: Simulated age (optional, not used in modeling)
- `NR2B`: NMDA receptor subunit expression
- `LTP`: Long-term potentiation strength
- `Synaptic_Density`: Modeled synaptic growth
- `Memory_Score`: Simulated memory performance outcome

Noise was added at each level to mimic real-world biological variability.

---

## 🤖 Model Summary

- Model: Multi-Layer Perceptron Regressor (sklearn)
- Input features:  
  `['Brain_Mg', 'Estrogen', 'BDNF', 'NR2B', 'LTP', 'Synaptic_Density']`
- Output: `Memory_Score`
- Performance Metric: Mean Squared Error (MSE)
- Feature Importance: Computed via permutation importance

---

## 🔍 Key Findings

- **Brain Magnesium** was the most predictive input for memory performance, acting as an upstream driver of the entire system.
- **Synaptic Density** held strong predictive value as the final step before memory.
- Intermediate factors like **NR2B**, **LTP**, **Estrogen**, and **BDNF** showed lower importance due to redundancy in the model — not lack of biological relevance.

---

## 🧪 Why This Project Matters

This project demonstrates how AI and synthetic modeling can be used to:
- Explore cognitive mechanisms with zero real-world risk
- Identify meaningful biological variables
- Simulate how nootropics like Magnesium L-Threonate may work on a systems level

---

## 🚀 Next Steps

Future simulations may explore:
- L-Theanine + Caffeine (attention and arousal)
- Lion’s Mane (BDNF and neurogenesis)
- Bacopa Monnieri (delayed memory consolidation)
- Dopamine-focused pathways for motivation and flow

---


## 🚀 Author
Daivarsi Malik  
[Instagram: @cognitive.engineer](https://instagram.com/cognitive.engineer)  
PhD-track Biomedical Engineer | Applied AI | Cognitive Neuroscience Modeling  

> This is an educational project. It is not intended for clinical or diagnostic use.
