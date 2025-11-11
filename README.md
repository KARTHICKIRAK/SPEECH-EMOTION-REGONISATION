# Multi-Feature CNN-GRU Framework for Speech Emotion Recognition

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)](https://www.tensorflow.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

A robust and accurate Speech Emotion Recognition (SER) system that identifies human emotions from speech signals using a hybrid CNN-GRU architecture. The system leverages multiple audio features — MFCCs, Spectrograms, and Cochleagrams — to capture complementary aspects of emotional speech, resulting in higher accuracy and noise robustness.

## 🎯 Objective

- Preprocess and standardize speech signals for consistent analysis
- Extract multiple audio features (MFCCs, Spectrograms, Cochleagrams)
- Design and implement a CNN–GRU model to capture spatial and temporal patterns
- Evaluate performance using benchmark emotion datasets
- Develop a lightweight, scalable system suitable for real-time applications

## 🏗️ System Architecture

```
Speech Input → Preprocessing → Feature Extraction → Feature Fusion → CNN + GRU Model → Emotion Output
```

### 🔑 Key Components

- **CNN**: Extracts spatial patterns from time–frequency representations
- **GRU**: Models temporal dependencies for dynamic emotion transitions  
- **Feature Fusion**: Combines multiple representations for improved accuracy and generalization

## 📋 Requirements

### Software Requirements

- **Programming Language**: Python 3.7+
- **Frameworks**: TensorFlow / PyTorch
- **Libraries**:
  - `librosa` – Audio feature extraction
  - `numpy`, `pandas`, `matplotlib` – Data handling and visualization
  - `scikit-learn` – Evaluation and metrics
- **Development Environment**: Google Colab / Jupyter Notebook
- **Version Control**: GitHub

### Installation

```bash
pip install tensorflow librosa numpy pandas matplotlib scikit-learn
```

## 📊 Dataset

The model can be trained and validated on publicly available emotion datasets:

- **RAVDESS** – Ryerson Audio-Visual Database of Emotional Speech and Song
- **TESS**, **SAVEE**, or **EMO-DB** (optional alternatives)

## 🚀 Implementation

### 1. Data Collection & Preprocessing
- Load dataset, remove noise, normalize signals
- Segment and label emotion classes

### 2. Feature Extraction
- Extract MFCCs, Spectrograms, and Cochleagrams using librosa

### 3. Feature Fusion
- Concatenate or merge features into a unified representation

### 4. Model Design
- Build hybrid CNN-GRU model in TensorFlow/PyTorch
- Use CNN layers for feature maps and GRU layers for sequential dependencies

### 5. Training & Evaluation
- Train model using categorical cross-entropy loss
- Evaluate accuracy, precision, recall, and F1-score

### 6. Deployment
- Deploy lightweight model for real-time inference on mobile/IoT devices

## 🛠️ Justification for Tools

- **Python**: Simplicity and vast ML ecosystem
- **TensorFlow/PyTorch**: GPU-accelerated model development
- **Librosa**: Reliable for extracting acoustic and frequency-based features
- **Google Colab**: Enables fast experimentation with cloud GPUs
- **GitHub**: Supports version control and collaborative tracking

## 📈 Results & Conclusion

The proposed system achieves enhanced emotion recognition accuracy through multi-feature fusion and hybrid deep learning. Compared to traditional single-feature CNN models, the CNN-GRU fusion improves robustness across speakers and noisy environments.

## 💡 Applications

- Healthcare monitoring
- Human–computer interaction
- Virtual assistants
- Emotion-aware learning systems

## 📚 References

Key references include works on CNN-GRU hybrid models, multi-feature fusion, and benchmark datasets such as RAVDESS and BanglaSER.

---

**Note**: This project is under active development. Contributions and suggestions are welcome!

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
