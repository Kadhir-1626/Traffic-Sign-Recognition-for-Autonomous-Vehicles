# Traffic-Sign-Recognition-for-Autonomous-Vehicles
# 🚦 Traffic Sign Recognition for Autonomous Vehicles

A deep learning project that detects and classifies traffic signs using Convolutional Neural Networks (CNNs). This system is built for integration into autonomous vehicle systems to help interpret road signage in real-time.

![Traffic Sign Recognition](https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/German_traffic_signs_collage.jpg/800px-German_traffic_signs_collage.jpg)

---

## 📌 Table of Contents
- [About the Project](#about-the-project)
- [Demo](#demo)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Future Work](#future-work)
- [License](#license)

---

## 📖 About the Project

Autonomous vehicles must detect and understand traffic signs to operate safely. This project trains a CNN model on the German Traffic Sign Recognition Benchmark (GTSRB) dataset to recognize 43 different types of traffic signs with high accuracy.

---

## 🎥 Demo

Check out a short demo of the model classifying real-time traffic signs (if available):

> _Upload or link to a video demo, GIF, or images of the working model._

---

## 📊 Dataset

- **Name:** German Traffic Sign Recognition Benchmark (GTSRB)
- **Size:** ~50,000 images
- **Classes:** 43 types of traffic signs
- **Source:** [GTSRB on Kaggle](https://www.kaggle.com/datasets/valentynsichkar/traffic-signs-preprocessed)

---

## 🛠 Technologies Used

- Python 3.8+
- TensorFlow / Keras
- NumPy & Pandas
- OpenCV
- Scikit-learn
- Matplotlib & Seaborn
- Flask (for deployment - optional)

---

## ⚙️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/traffic-sign-recognition.git
   cd traffic-sign-recognition
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download the dataset** (if not already included):
   - Place dataset in the `data/` directory.

---

## 🚀 Usage

### Training the Model
```bash
python train.py
```

### Testing the Model
```bash
python test.py
```

### Predicting a New Image
```bash
python predict.py --image path_to_image.jpg
```

### Running Web Interface (Optional)
```bash
python app.py
```

Then open your browser at `http://localhost:5000`

---

## 🧠 Model Architecture

- Convolutional Neural Network (CNN)
- Architecture:
  - Conv2D → ReLU → MaxPooling → Dropout
  - Fully Connected Layers
  - Softmax Output (43 classes)

- Optimizer: Adam
- Loss: Categorical Crossentropy
- Epochs: 30
- Accuracy Achieved: ~95% on test set

---

## 📈 Results

| Metric     | Value     |
|------------|-----------|
| Train Acc  | 98.5%     |
| Test Acc   | 94.8%     |
| Model Size | ~10 MB    |

- Confusion matrix, classification report, and visualized predictions are available in the `/results` folder.

---

## 🔮 Future Work

- Deploy on Raspberry Pi for real-time inference
- Enhance robustness under poor lighting/weather conditions
- Add multilingual sign detection (e.g., stop signs in different languages)
- Integrate with autonomous driving simulation (e.g., CARLA)

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

- [GTSRB Dataset](https://benchmark.ini.rub.de/gtsrb_news.html)
- TensorFlow/Keras documentation
- [OpenCV](https://opencv.org/)

---

## ✉️ Contact

If you have any questions or suggestions, feel free to open an issue or reach out:

**Your Name**  
📧 your.email@example.com  
🌐 [LinkedIn](https://www.linkedin.com/in/your-profile)
