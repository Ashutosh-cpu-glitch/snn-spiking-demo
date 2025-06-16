Spiking Neural Network (SNN) Demo for MNIST Classification 🧠💡
Welcome to my first-ever GitHub project—a Spiking Neural Network (SNN) implementation for classifying handwritten digits from the MNIST dataset, built using the Norse library in PyTorch! This project dives into the fascinating world of neuromorphic computing, mimicking how biological neurons communicate through spikes. As a beginner in SNNs, I created this to explore Leaky Integrate-and-Fire (LIF) neurons and spatio-temporal learning, achieving ~90%+ accuracy on MNIST. 🚀
🌟 Project Highlights

Neuromorphic Approach: Uses spiking neurons (LIF) for energy-efficient, brain-inspired digit classification.
Tech Stack: Built with Norse (for SNN primitives), PyTorch (for GPU acceleration), and torchvision (for MNIST).
Beginner-Friendly: Simple codebase designed to help others learn SNN basics.
Performance: Achieves ~90%+ test accuracy after 10 epochs on MNIST.

🧪 What Are Spiking Neural Networks?
Unlike traditional neural networks, SNNs process information using discrete spikes over time, similar to how neurons work in the human brain. This makes them ideal for energy-efficient computing and neuromorphic hardware like Intel's Loihi. In this project, I use LIF neurons to encode and classify MNIST digits, leveraging Norse's PyTorch-based framework for seamless integration.
📦 Installation
Get started in a few simple steps!

Clone the Repository:
git clone https://github.com/Ashutosh-cpu-glitch/snn-spiking-demo.git
cd snn-spiking-demo


Install Dependencies:Ensure you have Python 3.8+. Install required packages using:
pip install -r requirements.txt

Note: A compatible GPU is optional but recommended for faster training.

Download MNIST:The dataset is automatically downloaded via torchvision when you run the script.


🚀 Usage
Train and evaluate the SNN with a single command:
python src/snn_mnist.py --data-dir ./data --epochs 10 --batch-size 64

Expected Output

Training logs showing loss and accuracy per epoch.
Final test accuracy (~90%+ after 10 epochs).
Model weights can be saved to outputs/ (optional feature).

📂 Project Structure
├── README.md              # Project documentation
├── requirements.txt       # Dependencies
├── src/
│   ├── snn_mnist.py       # Main script for training and evaluation
├── data/                  # MNIST dataset (auto-downloaded)
├── outputs/               # Saved models and plots (optional)

🛠️ How It Works

Data Encoding: MNIST images are converted into spike trains using rate-based encoding.
SNN Architecture: A feedforward network with LIF neurons processes spatio-temporal data.
Training: Uses surrogate gradient descent (via Norse) to optimize weights.
Evaluation: Computes accuracy on the MNIST test set.

🔮 Future Improvements
As my first project, this is a starting point! Potential enhancements include:

Adding visualizations for spike trains and membrane potentials.
Supporting other datasets (e.g., FashionMNIST).
Exploring advanced SNN techniques like STDP (Spike-Timing-Dependent Plasticity).
Adapting for neuromorphic hardware (e.g., Intel Loihi).

🤝 Contributing
Feedback and contributions are welcome! To contribute:

Fork the repository.
Create a feature branch (git checkout -b feature/YourFeature).
Submit a pull request with a clear description.

📜 License
This project is licensed under the MIT License. See LICENSE for details.
🙌 Acknowledgments

Norse: For an awesome PyTorch-based SNN framework.
PyTorch: For making deep learning accessible.
MNIST: The classic dataset for testing ML models.


🌍 Connect with Me!Loved this project? Check out my GitHub for more, or reach out on LinkedIn to discuss neuromorphic computing, ML, or just geek out about tech! 😄
This project was my first step into the exciting world of SNNs—hope it inspires you to explore neuromorphic computing too!
