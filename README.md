# 🧠 Deep Learning Projects

A collection of practical **Deep Learning and Computer Vision projects** built while learning and experimenting with neural networks, transfer learning, audio classification, and image classification.

The repository is organized as a collection of independent projects, with each project containing its own notebook, trained model, supporting files, and documentation where applicable.

---

## 📌 Projects

| Project | Domain | Model / Approach | Task |
|---|---|---|---|
| 🐾 [Animal Classifier](animal_classifier/) | Computer Vision | EfficientNetB0 + Transfer Learning | 80-class animal image classification |
| 🎙️ [Audio Deepfake Detection](audio_deepfake/) | Audio / Deep Learning | CNN + Mel Spectrograms | Real vs Fake audio classification |
| 🧍 [Human Posture Recognition](human_posture_recognition/) | Computer Vision | MobileNetV2 + Transfer Learning | 4-class human posture classification |

---

## 🐾 1. Animal Classifier

An image classification project that recognizes **80 different animal classes**.

### Approach

- Pretrained **EfficientNetB0**
- Transfer learning
- Fine-tuning of later layers
- Global Average Pooling
- Dropout
- Softmax classification

### Workflow

```text
Input Image
     ↓
Resize to 224 × 224
     ↓
Pretrained EfficientNetB0
     ↓
Global Average Pooling
     ↓
Dropout
     ↓
Dense Classification Layer
     ↓
Animal Prediction
```

### Included

- Training notebook
- Trained `.h5` model
- Class-name mapping
- Sample images
- Accuracy and loss plots

👉 **[Open Animal Classifier](animal_classifier/)**

---

## 🎙️ 2. Audio Deepfake Detection

A deep learning project that classifies audio recordings as **Real** or **Fake**.

Raw audio is converted into **Mel Spectrograms**, which are then processed by a CNN.

### Approach

- Audio preprocessing with **Librosa**
- Resampling to 16 kHz
- Fixed 4-second audio segments
- 128-bin Mel Spectrogram
- CNN-based classification
- Sigmoid output for binary classification

### Workflow

```text
Audio File
    ↓
Load & Resample
    ↓
Pad / Trim to 4 Seconds
    ↓
Mel Spectrogram
    ↓
CNN
    ↓
Sigmoid
    ↓
Real / Fake
```

### Current Baseline

The current experiment was trained for 2 epochs.

- Training accuracy: **90.65%**
- Validation accuracy: **94.29%**
- Test accuracy: **84.18%**
- Parameters: **3,304,193**

These results belong to the current dataset and experiment and are not intended to represent universal real-world deepfake detection performance.

👉 **[Open Audio Deepfake Detection](audio_deepfake/)**

---

## 🧍 3. Human Posture Recognition

An image classification project that recognizes four human postures:

- 🧎 Bending
- 🛌 Lying
- 🪑 Sitting
- 🧍 Standing

### Approach

- Pretrained **MobileNetV2**
- ImageNet pretrained weights
- Transfer learning
- Fine-tuning of the final layers
- Global Average Pooling
- Dropout
- Softmax classification

### Workflow

```text
Posture Image
      ↓
Image Preprocessing
      ↓
MobileNetV2
      ↓
Global Average Pooling
      ↓
Dropout
      ↓
Softmax
      ↓
Posture Prediction
```

### Current Results

- Training accuracy: **92.50%**
- Validation accuracy: **90.83%**
- Validation loss: **0.2522**

👉 **[Open Human Posture Recognition](human_posture_recognition/)**

---

## 🛠️ Technologies Used

### Programming & Development
- Python
- Jupyter Notebook
- Google Colab

### Deep Learning
- TensorFlow
- Keras
- Convolutional Neural Networks (CNNs)
- Transfer Learning
- Fine-Tuning

### Computer Vision
- EfficientNetB0
- MobileNetV2
- Image Classification

### Audio Processing
- Librosa
- Mel Spectrograms
- Audio Classification

### Data & Visualization
- NumPy
- Matplotlib

---

## 📂 Repository Structure

```text
Deep-Learning-Projects/
│
├── animal_classifier/
│   ├── figures/
│   ├── models/
│   ├── class_names.json
│   ├── main.ipynb
│   └── README.MD
│
├── audio_deepfake/
│   ├── main.ipynb
│   ├── audio_deepfake_detector.keras
│   └── README.md
│
├── human_posture_recognition/
│   ├── figures/
│   ├── class_names.json
│   ├── main.ipynb
│   ├── posture_classifier.h5
│   └── README.md
│
└── README.md
```

---

## 🎯 Purpose

This repository is a growing collection of hands-on deep learning projects created to practice:

- Neural network development
- CNN architectures
- Transfer learning
- Fine-tuning pretrained models
- Image classification
- Audio classification
- Dataset preprocessing
- Model evaluation
- Model saving and loading
- Building reproducible machine learning workflows

More projects and experiments will be added over time.

---

## 👨‍💻 Author

**Deep Vejpara**

GitHub: [@Deepvejpara](https://github.com/Deepvejpara)

---

⭐ **Explore the individual project folders for detailed documentation, notebooks, trained models, datasets, and results.**
