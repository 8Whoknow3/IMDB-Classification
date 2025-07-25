# 🎬 IMDb Sentiment Analysis

An end-to-end project comparing traditional machine learning approaches and deep learning models for sentiment classification on the IMDb movie reviews dataset.

✅ Implements TF-IDF, Bag-of-Words, GLoVe embeddings, and neural networks (RNN, LSTM, Bidirectional LSTM)
✅ Provides training curves, evaluation metrics, and pre-trained models
✅ Includes reproducible Jupyter notebooks with clean visualizations


---

## 📂 Project Structure
```

├── IMDB-V1.ipynb       # Traditional ML models + GLoVe-based neural network
├── IMDB-V2.ipynb       # RNN & LSTM-based deep learning models
├── images/             # Visualizations and plots
└── README.md

````

### 🔗 Pre-trained Models
📥 [Download Pre-trained Models](https://drive.google.com/drive/folders/138NxQ50Kd_OlTcte5ixgT-17r5JRY2yr?usp=sharing)  
Models should be placed in the project directory in "models" folder for evaluation or fine-tuning.

---

## 📘 Notebook 1 – Traditional Models & GLoVe Embeddings
This notebook compares **TF-IDF**, **Bag-of-Words**, and **GLoVe embeddings with a neural network**.

| Model   | Test Accuracy | Test F1 Score | Best Validation F1 |
|---------|--------------|--------------|--------------------|
| TF-IDF  | 0.8512       | 0.8519       | 0.8846             |
| BoW     | 0.8568       | 0.8537       | 0.8822             |
| **GLoVe** | **0.8721** | **0.8707**   | **0.8956**         |

✅ **Result:** GLoVe embeddings achieved the **best overall performance**, outperforming traditional TF-IDF and BoW models.

---

## 📗 Notebook 2 – Deep Learning Models (RNN/LSTM)
This notebook evaluates **RNN**, **Bidirectional RNN**, **LSTM**, and **Bidirectional LSTM**.

| Model               | Best Val F1 | Test F1 | Test Accuracy |
|---------------------|------------|---------|---------------|
| RNN                 | 0.6168     | 0.6156  | 0.5048        |
| RNN (Bidirectional) | 0.7432     | 0.7173  | 0.7061        |
| LSTM                | 0.8367     | 0.8238  | 0.8182        |
| **LSTM (Bidirectional)** | **0.8381** | 0.8159  | **0.8193**    |

✅ **Result:** LSTM-based models significantly outperform RNNs.  
📌 **Bidirectional LSTM** achieves the **best validation F1**, while **LSTM performs similarly on test metrics**.

---

## 🚀 Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/8Whoknow3/IMDB-Classification.git
cd IMDB-Classification
````

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Download pre-trained models

Download from [Google Drive](https://drive.google.com/drive/folders/138NxQ50Kd_OlTcte5ixgT-17r5JRY2yr?usp=sharing) and place them in the project folder.

### 4️⃣ Run the notebooks

```bash
jupyter notebook IMDB-V1.ipynb
jupyter notebook IMDB-V2.ipynb
```

---

## 📊 Outputs

* **Training curves and evaluation plots** → stored in the `images/` folder
* **Saved models** → available on Google Drive

---

## 📝 Notebook Overview

| Notebook    | Content                                              |
| ----------- | ---------------------------------------------------- |
| **IMDB-V1** | TF-IDF, BoW, and GLoVe embedding comparison          |
| **IMDB-V2** | RNN, Bidirectional RNN, LSTM, and Bidirectional LSTM |

---

## 🔥 Key Takeaways

✅ **Traditional ML** methods are fast but limited in performance.
✅ **GLoVe embeddings** significantly boost classification results.
✅ **LSTM-based models** provide the **best generalization**, especially with bidirectional layers.

