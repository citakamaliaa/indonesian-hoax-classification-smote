# Indonesian Hoax Classification with SMOTE Optimization
This study evaluates the performance of five deep learning architectures combined with **SMOTE-based oversampling strategies** (Borderline-SMOTE, KMeans-SMOTE, SVM-SMOTE) and a proposed **Margin Loss function** and **Binary-Crossnetropy Loss function** to handle class imbalance in Indonesian hoax news classification.

## Project Overview
- **Dataset:**
  The dataset is available for download.
  [https://drive.google.com/drive/folders/1RLM-C7nxKE82CREzKb2QVr5VA5-J5f8Z?usp=sharing]
- **Embeddings:** Hybrid features using **IndoBERT** (Transformer) and **Word2Vec**.
- **Imbalance Handling:** Implemented three variants of SMOTE to address data scarcity in the minority class.
- **Loss Functions:** Compared standard **Binary Crossentropy** and **Margin Loss**.

The repository relies on Jupyter Notebooks (`.ipynb`) to ensure transparency of the training process, logs, and visualization. Each notebook represents a specific model architecture and loss function configuration.

**Clone the repository:**
   ```bash
   git clone [https://github.com/citakamaliaa/hoax-news-classification.git](https://github.com/citakamaliaa/hoax-news-classification.git)
   cd hoax-news-classification
```

## Install dependencies
It is recommended to use a virtual environment or Google Colab.
 ```bash
pip install -r requirements.txt
```

## Usage Instructions
Since the code is provided in Jupyter Notebook format, you can run the experiments interactively.

1. Choose a Scenario: Select the notebook corresponding to the model and loss function you wish to evaluate (see the table above).
2. Open the Notebook:
   - Local: Run jupyter lab or jupyter notebook in your terminal and open the file.
   - Cloud: Upload the .ipynb file to Google Colab.
3. Load Data:
  - Ensure the dataset (.csv) is placed in the correct directory as specified in the notebook, or upload it to the Colab session.
  - The notebooks include scripts (gdown) to automatically download the pre-trained Word2Vec model (idwiki_word2vec_768_new_lower.model).
4. Run All Cells: Execute the cells sequentially to perform preprocessing, SMOTE oversampling, training, and evaluation.

## Evaluation
The notebooks automatically generate the following metrics after training:
- Classification Report: Precision, Recall, F1-Score (Macro & Weighted).
- Confusion Matrix: Visualization of True Positives, False Positives, etc.
- Training Logs: Graphs showing Accuracy and Loss over epochs.

## Citation

## License
This project is licensed under the MIT License.
