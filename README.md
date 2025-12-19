# Indonesian Hoax Classification with SMOTE Optimization
This study evaluates the performance of five deep learning architectures combined with **SMOTE-based oversampling strategies** (Borderline-SMOTE, KMeans-SMOTE, SVM-SMOTE) and a proposed **Margin Loss function** and **Binary-Crossnetropy Loss function** to handle class imbalance in Indonesian hoax news classification.

## Project Overview
- **Dataset:**
  The dataset is available for download.
  [https://drive.google.com/drive/folders/1RLM-C7nxKE82CREzKb2QVr5VA5-J5f8Z?usp=sharing]
- **Embeddings:** Hybrid features using **IndoBERT** (Transformer) and **Word2Vec**.
- **Imbalance Handling:** Implemented three variants of SMOTE to address data scarcity in the minority class.
- **Loss Functions:** Compared standard **Binary Crossentropy** and **Margin Loss**.

The repository is organized into directories based on the experimental pipeline:
├── Preprocessing/ # Scripts/Notebooks for initial text cleaning ├── Dataset 1/ # Experiments using Dataset 1 (Balanced/Imbalanced scenarios) ├── Dataset 2/ # Experiments using Dataset 2 ├── Dataset 3_Test/ # Testing data and evaluation scripts ├── requirements.txt # Dependencies └── README.md # Project Documentation

## Usage Instructions

To reproduce the experiments, please follow these steps:

### 1. Clone the repository
```bash
git clone [https://github.com/citakamaliaa/indonesian-hoax-classification-smote.git](https://github.com/citakamaliaa/indonesian-hoax-classification-smote.git)
cd indonesian-hoax-classification-smote
```
### 2. Install dependencies
It is recommended to use a virtual environment or Google Colab.
```bash
pip install -r requirements.txt
```
### 3. Download Dataset
Due to file size limits, the dataset is hosted externally.
- Download the .csv files.
- Place the dataset files into the root directory or upload them to your Google Colab session.

### 4. Run Text Preprocessing
Navigate to the Preprocessing/ directory and execute the notebook to clean the raw data and prepare it for feature extraction.

### 5. Apply SMOTE and Train Models
Navigate to either Dataset 1/ or Dataset 2/ depending on the scenario you wish to test.
- Open the specific notebook (e.g., Berita_data_IndoBERT_MarginLoss.ipynb).
- Run the cells to apply SMOTE, Borderline-SMOTE, KMeans-SMOTE, or SVM-SMOTE and train the Deep Learning models (IndoBERT-CNN, LSTM, etc.).

### 6. Evaluate Model Performance
The evaluation steps are integrated within the training notebooks. Running the final cells will generate:
- Classification Report: Precision, Recall, F1-Score.
- Confusion Matrix.
- Loss & Accuracy Curves.

(Note: Validation on the separate test set can be performed using the files in the Dataset 3_Test/ directory).

## Citation

## License
This project is licensed under the MIT License.
