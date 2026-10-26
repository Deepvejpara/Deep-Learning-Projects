# 🧠 Deep Learning Projects

A collection of practical **Deep Learning, Computer Vision, and Audio AI projects** built while learning and experimenting with neural networks, image processing, transfer learning, CNNs, and audio classification.

The repository is organized into independent projects. Each project may include its own notebook, trained model, visualizations, supporting files, and documentation.

---

## 📌 Projects

| Project | Domain | Model / Approach | Task |
|---|---|---|---|
| 🖼️ [CIFAR-10 CNN & Image Processing](Project_A/) | Computer Vision | CNN, Convolution, Pooling | CIFAR-10 image classification and image-processing experiments |
| 🐾 [Animal Classifier](animal_classifier/) | Computer Vision | EfficientNetB0 + Transfer Learning | 80-class animal image classification |
| 🎙️ [Audio Deepfake Detection](audio_deepfake/) | Audio / Deep Learning | CNN + Mel Spectrograms | Real vs Fake audio classification |
| 🧍 [Human Posture Recognition](human_posture_recognition/) | Computer Vision | MobileNetV2 + Transfer Learning | 4-class human posture classification |

---

## 🖼️ 1. CIFAR-10 CNN & Image Processing

A hands-on deep learning project exploring image processing operations and Convolutional Neural Networks using the **CIFAR-10 dataset**.

### Topics Covered

- CIFAR-10 dataset exploration and pixel intensity histograms
- Manual convolution and zero padding
- Convolutional feature maps
- Max pooling vs. average pooling
- CNN model training
- Training and validation curves
- Confusion matrix and misclassified samples

### Visualizations

**Pixel Intensity Histograms**

![CIFAR-10 Pixel Intensity Histograms](Project_A/plots/a1_3_pixel_histograms.png)

**Convolutional Feature Maps**

![CNN Feature Maps](Project_A/plots/a2_4_conv2d_feature_maps.png)

**CNN Training Curves**

![CNN Training Curves](Project_A/plots/a4_3_cnn_training_curves.png)

👉 **[Open CIFAR-10 CNN & Image Processing](Project_A/)**

---

## 🐾 2. Animal Classifier

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

## 🎙️ 3. Audio Deepfake Detection

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

## 🧍 4. Human Posture Recognition

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
- Image preprocessing and convolution operations
- EfficientNetB0
- MobileNetV2
- Image classification
- Pooling and feature extraction

### Audio Processing
- Librosa
- Mel Spectrograms
- Audio classification

### Data & Visualization
- NumPy
- Pandas
- Matplotlib

---

## 📂 Repository Structure

```text
Deep-Learning-Projects/
│
├── Project_A/
│   ├── plots/
│   ├── models/
│   ├── DL_PR4.ipynb
│   └── README.md
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
- CNN architectures and image processing
- Transfer learning and fine-tuning
- Image and audio classification
- Dataset preprocessing
- Model evaluation and visualization
- Model saving and loading
- Building reproducible machine learning workflows

More projects and experiments will be added over time.

---

## 👨‍💻 Author

**Deep Vejpara**

GitHub: [@Deepvejpara](https://github.com/Deepvejpara)

---

⭐ **Explore the individual project folders for detailed documentation, notebooks, visualizations, trained models, and results.**
