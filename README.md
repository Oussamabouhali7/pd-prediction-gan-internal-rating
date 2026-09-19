# GAN-Based Probability of Default Prediction Using Internal Credit Ratings

## 📌 Overview

This project focuses on predicting the **Probability of Default (PD)** using **internal credit ratings** and Machine Learning techniques.

The project follows the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** methodology, covering the complete data science lifecycle from business understanding to model deployment.

A major challenge addressed in this project is the **class imbalance between default and non-default clients**. To overcome this issue, a **Generative Adversarial Network (GAN)** is used to generate synthetic observations and rebalance the dataset before training the PD prediction models.

The final solution is deployed through an interactive **Streamlit application** for credit-risk analysis and Probability of Default prediction.

---

## 🎯 Objectives

The main objectives of this project are:

* Predict the **Probability of Default (PD)** of clients.
* Analyze the relationship between **internal credit ratings** and default risk.
* Address the imbalance between default and non-default clients.
* Generate synthetic observations using a **GAN-based resampling approach**.
* Compare model performance before and after GAN-based resampling.
* Develop Machine Learning models for credit-risk prediction.
* Evaluate model performance using credit-risk and classification metrics.
* Deploy the final solution through an interactive **Streamlit application**.

---

## 🔄 CRISP-DM Methodology

The project follows the six phases of the **CRISP-DM methodology**.

### 1. Business Understanding

The objective is to develop a predictive solution capable of estimating the Probability of Default of clients using internal credit ratings and borrower-related characteristics.

The solution can support:

* Credit risk assessment
* Risk segmentation
* Credit decision support
* Portfolio risk analysis
* Identification of high-risk clients

### 2. Data Understanding

The dataset contains information related to borrowers, including:

* Internal credit ratings
* Financial characteristics
* Client information
* Historical default information
* Risk-related variables

Exploratory Data Analysis (EDA) is performed to understand the dataset and identify relationships between variables and default behavior.

Particular attention is given to the distribution of **default and non-default clients**.

### 3. Data Preparation

The data preparation process includes:

* Data cleaning
* Missing-value treatment
* Duplicate detection
* Outlier analysis
* Categorical variable encoding
* Feature engineering
* Feature selection
* Data transformation
* Preparation of training and testing datasets

The class distribution is analyzed before applying the GAN-based resampling approach.

### 4. Modeling

Machine Learning models are trained to estimate the Probability of Default.

The modeling pipeline combines:

**Internal Credit Ratings + Financial Variables + Client Characteristics → Feature Engineering → GAN Resampling → PD Prediction**

The impact of GAN-based resampling is evaluated by comparing models trained on the original dataset with models trained on the resampled dataset.

### 5. Evaluation

The models are evaluated using several performance and credit-risk metrics:

* **ROC-AUC**
* **Gini Coefficient**
* **KS Statistic**
* **Accuracy**
* **Precision**
* **Recall**
* **F1-Score**
* **Brier Score**

The comparison allows the effectiveness of GAN-based data resampling to be assessed.

### 6. Deployment

The final solution is deployed using **Streamlit**, providing an interactive interface for exploring the data and obtaining Probability of Default predictions.

---

## 🤖 GAN-Based Data Resampling

Credit-risk datasets are often highly imbalanced, with significantly fewer default observations than non-default observations.

This imbalance can negatively affect Machine Learning models by causing them to favor the majority class.

To address this problem, a **Generative Adversarial Network (GAN)** is used to learn the underlying distribution of the data and generate synthetic observations.

### GAN Workflow

```text
Original Dataset
       ↓
Class Imbalance Analysis
       ↓
GAN Training
       ↓
Synthetic Data Generation
       ↓
GAN-Based Resampling
       ↓
Balanced Dataset
       ↓
PD Prediction Models
```

The generated synthetic observations are incorporated into the training process to improve the representation of the minority class.

---

## 🧠 Probability of Default Prediction

The **Probability of Default (PD)** represents the estimated likelihood that a borrower will default within a defined time horizon.

The project uses internal credit ratings together with borrower and financial characteristics to estimate this probability.

The complete prediction process is:

```text
Client Information
       ↓
Internal Credit Rating
       ↓
Data Preprocessing
       ↓
Feature Engineering
       ↓
GAN-Based Resampling
       ↓
Machine Learning Model
       ↓
Probability of Default
       ↓
Risk Assessment
```

---

## 🖥️ Streamlit Application

The developed **Streamlit application** provides an interactive interface for the PD prediction solution.

The application allows users to:

* Explore credit-risk data
* Analyze default and non-default distributions
* Examine internal credit ratings
* Visualize relevant variables
* Apply the trained prediction model
* Obtain Probability of Default estimates
* Analyze model performance

### Application Workflow

```text
User Input
    ↓
Preprocessing
    ↓
Feature Transformation
    ↓
Trained Model
    ↓
PD Prediction
    ↓
Risk Interpretation
```

---

## 🛠️ Technologies & Tools

### Programming

* Python
* Jupyter Notebook

### Data Processing

* Pandas
* NumPy

### Machine Learning

* Scikit-learn
* Machine Learning classification models

### Deep Learning

* Generative Adversarial Networks (GAN)

### Data Visualization

* Matplotlib
* Seaborn
* Plotly

### Deployment

* Streamlit

### Methodology

* CRISP-DM

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/pd-prediction-gan.git
cd pd-prediction-gan
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Streamlit Application

Launch the application with:

```bash
streamlit run app.py
```

The Streamlit interface will then be available locally in your browser.

---

## 📊 Results

The project evaluates the impact of GAN-based resampling on Probability of Default prediction.

The performance of models trained on the **original dataset** is compared with models trained on the **GAN-resampled dataset** using multiple evaluation metrics.

This approach provides insights into whether synthetic data generation can improve the identification of default clients and the overall performance of credit-risk models.

---

## 🏦 Credit Risk Context

Probability of Default is a fundamental component of **credit risk modeling** and plays an important role in assessing the creditworthiness of borrowers.

Internal credit ratings provide a structured way to differentiate borrowers according to their level of risk. Combining these ratings with financial and borrower characteristics enables the development of data-driven PD models.

The integration of **Machine Learning and GAN-based synthetic data generation** provides an alternative approach to handling imbalanced credit-risk datasets.

---

## 👨‍💻 Author

**Oussama Bouhali**

**Final Year Engineering Project (PFE)**
**Quantylix — Part of the PwC Network**

### Areas of Focus

* Credit Risk Modeling
* Probability of Default
* Internal Credit Ratings
* Machine Learning
* Generative Adversarial Networks
* Data Science
* CRISP-DM
* Streamlit Deployment

---

## ⚠️ Disclaimer

This project is intended for **academic, research, and educational purposes**. The models and predictions should not be used directly for real-world credit decisions without appropriate validation, model governance, regulatory compliance, and expert review.
