# 🧠 Spiking Neural Network (SNN) for MNIST Classification

Welcome to my first neuromorphic computing project—a Spiking Neural Network (SNN) designed to classify handwritten digits from the MNIST dataset using the **Norse** library built on top of **PyTorch**.

This project explores how **Leaky Integrate-and-Fire (LIF)** neurons process spatio-temporal information via discrete spikes, mimicking how biological neurons function. Achieving \~90%+ accuracy after 10 epochs, this serves as a beginner-friendly yet powerful entry into the world of **brain-inspired AI**.

---

## 🌟 Key Features

* **Neuromorphic Learning**: Leverages biologically-plausible LIF neurons for energy-efficient computation.
* **Modern Tech Stack**: Utilizes Norse (SNN primitives), PyTorch (GPU acceleration), and Torchvision (data utilities).
* **Educational Focus**: Designed with simplicity for beginners entering the SNN field.
* **High Accuracy**: Reaches \~90%+ test accuracy on MNIST with minimal tuning.

---

## 🔬 What Are Spiking Neural Networks (SNNs)?

Unlike traditional artificial neural networks that operate on continuous signals, **Spiking Neural Networks** transmit and process information using discrete spikes across time—just like real neurons. This allows for:

* Temporal coding of information
* Lower energy consumption
* Suitability for neuromorphic hardware (e.g., Intel Loihi)

In this project, we simulate LIF neuron behavior using Norse’s PyTorch extensions to classify digit images in a biologically realistic way.

---

## ⚙️ Installation Instructions

1. **Clone the Repository**

```bash
git clone https://github.com/Ashutosh-cpu-glitch/snn-spiking-demo.git  
cd snn-spiking-demo  
```

2. **Install Dependencies**
   Ensure Python ≥ 3.8 is installed. Then:

```bash
pip install -r requirements.txt
```

> *Note: A GPU is optional but recommended for training speed.*

3. **Download MNIST Dataset**
   Torchvision will automatically download MNIST on first run.

---

## 🚀 Run the Experiment

Execute the training and evaluation pipeline:

```bash
python src/snn_mnist.py --data-dir ./data --epochs 10 --batch-size 64
```

**Expected Output:**

* Epoch-wise training loss and accuracy
* Final test accuracy of \~90%+
* Model checkpoints (optional) in `outputs/` folder

---

## 📁 Project Structure

```
├── README.md               # Project overview and usage
├── requirements.txt        # Python dependencies
├── snn-spiking-demo.ipynb

              
```

---

## 🛠️ Methodology

* **Input Encoding**: Converts static images to spike trains using rate-based encoding.
* **SNN Architecture**: A feedforward structure built with LIF neurons processes the encoded input.
* **Training**: Surrogate gradient descent via Norse is used to train synaptic weights.
* **Evaluation**: Reports classification accuracy on MNIST test set.

---

## 🔮 Future Scope

This is just the beginning! Planned improvements include:

* Visualization of spike trains and membrane dynamics
* Support for additional datasets like FashionMNIST
* Integrating biologically-plausible rules (e.g., STDP)
* Porting to neuromorphic chips like **Intel Loihi**

---

## 🤝 Contributing

All contributions are welcome! To contribute:

```bash
1. Fork this repository  
2. Create a new branch: git checkout -b feature/YourFeature  
3. Commit your changes and push  
4. Open a pull request with a clear explanation
```

---

## 📜 License

This project is released under the **MIT License**. See [LICENSE](./LICENSE) for full text.

---

## 🙌 Acknowledgments

* **Norse**: For the spiking neuron modules
* **PyTorch**: For a powerful and flexible deep learning framework
* **MNIST Dataset**: A standard for benchmarking image classifiers

---

## 🌍 Connect with Me!

If this project sparked your curiosity in SNNs or neuromorphic computing, feel free to:

* 🌐 Explore more on my [GitHub](https://github.com/Ashutosh-cpu-glitch)
* 💼 Connect with me on [LinkedIn](#)
* 🤓 Let’s talk AI, brains, and beyond!

---

Ready to spike your neurons into the future of AI? Let’s build smarter, brain-like machines together. 🧠⚡

---


