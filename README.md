# Lung Cancer Classification with SVM and Random Forest

This Jupyter Notebook contains code for classifying lung cancer types (LUAD and LUSC) using Support Vector Machines (SVM) and Random Forest classifiers. The dataset used for this classification task is provided in the file `HW3Data_lncRNA_2_cancers.csv`.

## Dataset

The dataset contains gene expression data for long non-coding RNAs (lncRNAs) associated with two types of lung cancer: LUAD (Lung Adenocarcinoma) and LUSC (Lung Squamous Cell Carcinoma). Each row in the dataset represents a sample, and the columns represent different lncRNAs.

- **File**: `HW3Data_lncRNA_2_cancers.csv`
- **Size**: 1008 rows × 12311 columns
- **Number of Samples**: 1008
- **Data Format**: Comma-separated values (CSV)
- **Features**: Each feature represents the expression level of a specific lncRNA.
- **Target Variable (Class)**:
  - `LUAD`: Lung Adenocarcinoma (1)
  - `LUSC`: Lung Squamous Cell Carcinoma (0)

## Code Overview

The code performs the following steps:

1. Data Loading and Preprocessing: Reads the dataset and preprocesses it by removing unnecessary columns and encoding the target variable (Class) as binary (1 for LUAD and 0 for LUSC).
2. Data Splitting: Splits the dataset into training and testing sets.
3. Model Training: Trains SVM and Random Forest classifiers on the training data.
4. Model Evaluation: Evaluates the performance of the trained models using accuracy, confusion matrix, and ROC curve analysis.
5. Visualization: Visualizes the results using seaborn and matplotlib.

## Dependencies

- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn

## Usage

To run the code:

1. Install the required dependencies using pip:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn
```

Open the Jupyter Notebook in a Jupyter Notebook environment (e.g., Google Colab).
Execute the cells in the notebook sequentially.

##Output

The notebook generates the following outputs:

Confusion matrices for SVM and Random Forest classifiers.
ROC curves and AUC scores for both classifiers.
Classification reports displaying precision, recall, F1-score, and support for each class.
Visualization of the confusion matrices and ROC curves.
