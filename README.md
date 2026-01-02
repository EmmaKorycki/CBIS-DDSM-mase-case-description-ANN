# Breast Cancer Detection via Artificial Neural Networks (ANN)

This project focuses on improving the accuracy of breast cancer detection by analyzing mammography mass features. Using a neural network approach, the model predicts the probability of malignancy based on clinical descriptors.

## Dataset & Visualizations
The analysis utilizes the **CBIS-DDSM (Curated Breast Imaging Subset of DDSM)** mass-case-description dataset. Key exploratory data analysis (EDA) included:
* **Pathology Distribution:** Visualizing BI-RADS assessment scores (Malignant, Benign, Benign without callback).
* **Feature Analysis:** Mapping the count of malignant cases according to specific mass features (shape, margin, density).

## Model Architecture
The core model is an **Artificial Neural Network (ANN)** designed to classify breast masses.
* **Input Layer:** Features extracted from the mass-case-descriptions.
* **Architecture:** Used Keras Tuner to tune hyperparameters by random search.
* **Output Layer:** Sigmoid activation providing the probability of malignancy.

## Performance Results
The model demonstrated strong predictive capabilities, particularly in balancing precision and recall.

| Metric | Score |
| :--- | :--- |
| **Train Accuracy** | 87.87% |
| **Test Accuracy** | 78.97% |
| **Precision** | 78.21% |
| **Recall (Sensitivity)** | 79.01% |
| **F1-Score** | 78.45% |
| **False Positive Rate** | 20.99% |

<details>
<summary><b>Click to view Confusion Matrix Data</b></summary>



* **True Negatives:** 170 (Correctly identified benign)
* **False Positives:** 46 (Benign flagged as malignant)
* **False Negatives:** 30 (Malignant missed)
* **True Positives:** 115 (Correctly identified malignant)

</details>

## Getting Started
1. **Clone the Repo:** `git clone https://github.com/your-username/your-repo-name.git`
2. **Install Dependencies:** `pip install -r requirements.txt`
3. **Run Analysis:** Open the provided Jupyter Notebook to view the full pipeline.

---
*A slide presentation is included in this repository to provide further clinical context and project details.*

