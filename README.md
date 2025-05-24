## 🚦 Traffic Sign Classification using CNN (Keras/TensorFlow)

This project implements a Convolutional Neural Network (CNN) to classify traffic signs from the German Traffic Sign Recognition Benchmark (GTSRB) dataset. The goal is to enable automated recognition of road signs, a key step in developing self-driving car systems and advanced driver-assistance systems (ADAS).

---

### 📌 Key Features

* 🔍 **Image Classification** of 43 traffic sign classes
* 🧠 **Custom CNN architecture** designed for performance and faster training
* ⚙️ Built using **Keras with TensorFlow backend**
* 💡 Simplified model for faster execution without sacrificing much accuracy
* 📊 Includes training history visualization and validation performance

---

### 📁 Dataset

* The model is trained on the [GTSRB dataset](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset), a popular real-world traffic sign dataset consisting of over 50,000 labeled images of traffic signs captured under varying lighting and weather conditions.

---

### 🏗️ Model Architecture

```text
Input → Conv2D(32) → MaxPooling → Dropout
      → Conv2D(32) → MaxPooling
      → Flatten → Dense(64) → Dropout → Dense(43 softmax)
```

* Uses ReLU activation, softmax output
* Optimized with Adam optimizer
* Dropout added to reduce overfitting
* Batch size: 32 (recommended)

---

### 📈 Results

* Achieves high classification accuracy on validation and test sets
* Training time is optimized for general-purpose systems without GPU

---

### 🧪 How to Run

1. Clone the repo:

   ```bash
   git clone https://github.com/MahirHossain12/traffic-sign-classification.git
   cd traffic-sign-classification
   ```

2. Install requirements:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook or execute scripts:

   ```bash
   jupyter notebook Traffic_Sign_Classification.ipynb
   ```

---

### 🔮 Future Work

* Integrate real-time webcam prediction
* Improve model with transfer learning (e.g., MobileNetV2)
* Deployment using Flask/Streamlit or TensorFlow Lite

---

### 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

