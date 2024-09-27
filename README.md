# ensambleml

### `README.md`

```markdown
# Fetal Health Classification Project

## Overview
This project involves applying machine learning techniques to classify fetal health status using the "Fetal Health Classification" dataset. The dataset contains various features related to fetal health, and the goal is to distinguish between different fetal health conditions: Normal, Suspect, and Pathological.

## Dataset
The dataset used in this project is available on Kaggle: [Fetal Health Classification Dataset](https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification).

## Project Structure
- **Data Preprocessing:** The data was cleaned, normalized, and split into training and testing sets.
- **Model Training:**
  - **Random Forest:** Trained with 100, 300, and 1000 trees. The model with 1000 trees provided the best balanced accuracy.
  - **Gradient Boosting:** Trained with varying `n_estimators` (100 and 200) and `learning_rate` (0.01, 0.1, 1.0). The best results were obtained with 100 estimators and a learning rate of 0.1.
- **Model Evaluation:** Both models were evaluated using balanced accuracy, and the Gradient Boosting model was further assessed using ROC curves and AUC.
- **Final Analysis:** The Gradient Boosting model demonstrated excellent performance, with an AUC of 0.98 for the Normal class, 0.97 for the Suspect class, and 1.00 for the Pathological class.

## Results
- **Balanced Accuracy:**
  - Random Forest: Best balanced accuracy of 0.9095 with 1000 trees.
  - Gradient Boosting: Best balanced accuracy of 0.9212 with 100 estimators and a learning rate of 0.1.
- **ROC and AUC:** The ROC curves and AUC values indicated strong performance across all classes, particularly for the Pathological class, which achieved an AUC of 1.00.

## Getting Started

### Prerequisites
To run the code, you will need the following Python libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `seaborn`
- `matplotlib`

### Installation
You can install the necessary packages using pip:
```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```

### Running the Project
1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd assignments
   ```

2. **Prepare the dataset:**
   - Download the dataset from Kaggle and place the `fetal_health.csv` file in the project directory.

3. **Run the Jupyter Notebook or Python script:**
   - Load the dataset, preprocess it, and run the training and evaluation code to reproduce the results.

### File Descriptions
- `fetal_health.csv`: The dataset used for training and evaluation.
- `notebook.ipynb`: The main code file or notebook containing all steps from data loading to model evaluation.
- `README.md`: This file, explaining the project structure and how to get started.
