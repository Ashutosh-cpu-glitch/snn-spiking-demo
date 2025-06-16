# snn-spiking-demo
# 🧠 Neuromorphic Spike-Based Simulation using Leaky Integrate-and-Fire Neuron

This repository presents a scientific, interpretable implementation of a **spiking neural network (SNN)** using the **Leaky Integrate-and-Fire (LIF)** neuron model. The project simulates biologically inspired neuron dynamics and spike-based decision-making using Python and Jupyter Notebook, offering an educational and research-aligned introduction to **neuromorphic computing**.

---

## 📌 Abstract

Neuromorphic computing seeks to mimic the brain's event-driven architecture using spiking neuron models that communicate via discrete action potentials (spikes). Unlike conventional neural networks, SNNs encode information temporally, enabling asynchronous and low-power computation.

This project demonstrates the temporal dynamics of a single LIF neuron receiving input from synthetic stimuli. The goal is to model how such neurons integrate inputs, leak membrane potential over time, and emit spikes when a threshold is exceeded — a fundamental process in biological neural systems.

---

## 🔬 Methodology

- **Neuron Model**: Leaky Integrate-and-Fire (LIF)
- **Simulation Framework**: Python + NumPy
- **Input**: 2D synthetic blob data (via scikit-learn)
- **Encoding**: Rate-based spike encoding from continuous input
- **Processing**: Temporal membrane integration and spike generation
- **Output Decision**: Classification via total spike count across simulation window

---

## 🧠 Biological Analogy

| Model Component         | Biological Equivalent       |
|-------------------------|-----------------------------|
| Membrane potential `V`  | Post-synaptic potential     |
| Leak constant `α`       | Passive voltage decay       |
| Threshold `θ`           | Action potential trigger    |
| Spike event             | Neuronal firing             |
| Time steps              | Discrete simulation of time |

---

## 📊 Features

- Biologically plausible LIF neuron
- Temporal simulation of spike trains
- Synthetic input encoding and visualization
- Classification using spike frequency
- All logic written from scratch (no deep learning frameworks)

---

## 📦 Dependencies

Install the required packages using:

```bash
pip install numpy matplotlib scikit-learn notebook
## 💻 Run
jupyter notebook snn_spike_demo.ipynb
## License
This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
