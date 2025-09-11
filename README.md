🖼️ CIFAR-10 Image Classification with CNN

This project demonstrates how to build and train a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify images from the CIFAR-10 dataset.
The CIFAR-10 dataset consists of 60,000 images (32x32, RGB) across 10 categories:

🚀 Airplane | 🚗 Automobile | 🐦 Bird | 🐱 Cat | 🦌 Deer | 🐶 Dog | 🐸 Frog | 🐴 Horse | 🚢 Ship | 🚚 Truck

📂 Project Workflow

1️⃣ Data Loading

Load CIFAR-10 from tensorflow.keras.datasets.

Train/Test split → 50,000 / 10,000 samples.

2️⃣ Preprocessing

Normalize pixel values → [0, 1].

Keep labels as integers (0–9).

3️⃣ Model Architecture 🧠

Conv2D + ReLU + MaxPooling layers

Dense (fully connected) layers with ReLU

Dropout for regularization

Softmax output layer for classification

4️⃣ Training

Optimizer: Adam

Loss: Sparse Categorical Crossentropy

Epochs: 10

Batch size: 64

5️⃣ Evaluation & Visualization

Accuracy & loss plots over epochs

Model evaluation on test set

Predictions visualized (True vs Predicted labels)

🎯 CIFAR-10 Classes
Label	Class	Emoji
0	Airplane	✈️
1	Automobile	🚗
2	Bird	🐦
3	Cat	🐱
4	Deer	🦌
5	Dog	🐶
6	Frog	🐸
7	Horse	🐴
8	Ship	🚢
9	Truck	🚚
📊 Results

✔️ Training Accuracy improves steadily across epochs
✔️ Validation Accuracy ~70–80% (with default CNN)
✔️ Handles most categories well, some confusion in Cat vs Dog

📈 Example Accuracy/Loss Curves:

(insert your plot images here)

🔍 Example Predictions
True: Dog 🐶   → Pred: Dog ✅  
True: Cat 🐱   → Pred: Dog ❌  
True: Airplane ✈️ → Pred: Airplane ✅  

🛠️ How to Run

Clone the repo and run the notebook:

git clone https://github.com/musfira512/cifar10-cnn.git
cd cifar10-cnn
jupyter notebook


Or run the script:

python cifar10_cnn.py

🤝 Acknowledgements

Dataset: CIFAR-10

Framework: TensorFlow / Keras
