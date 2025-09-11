# 🧠📊 Synthetic Data Generator using GANs

[![Python](https://img.shields.io/badge/python-v3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow](https://img.shields.io/badge/tensorflow-v2-orange.svg)](https://www.tensorflow.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange.svg)](https://scikit-learn.org/)
[![pandas](https://img.shields.io/badge/pandas-Data%20Wrangling-150458.svg)](https://pandas.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A complete synthetic data generation solution using Generative Adversarial Networks (GANs) to create privacy-safe synthetic app usage data. Built with Python, TensorFlow, and scikit-learn, perfect for data augmentation and safe model training.

---

## ✨ Features

- 📤 Upload & Manage Data  
  Upload your app usage dataset in CSV format using Google Colab file uploader.

- 🧹 Data Preprocessing  
  Drop unneeded columns, normalize numeric data using MinMaxScaler.

- ⚙️ Generator & Discriminator Models  
  Fully configured Keras-based Generator and Discriminator architectures for synthetic data generation.

- 🔄 Adversarial Training  
  Train GAN in an adversarial setup for realistic synthetic data generation.

- 💾 Model Persistence  
  Save generator model (`generator.h5`), scaler (`scaler.pkl`), and column mapping (`columns.json`) for reuse.

- 📊 Generate Synthetic Samples  
  Generate and export new synthetic records after training.

---

## 🚀 Quick Start

```bash
# Clone this repo
git clone https://github.com/your-username/gan-synthetic-data-generator.git
cd gan-synthetic-data-generator

# Open in Google Colab
# Upload your 'screentime_analysis.csv'

# Install required dependencies
pip install -r requirements.txt

# (Optional) Install huggingface tools
pip install huggingface_hub
apt-get install git-lfs -y
git lfs install

# Run the notebook in Google Colab
# Step by step run cells to preprocess data, build models, train GAN, and generate synthetic data

# After training:
# generator.h5, scaler.pkl, columns.json will be saved automatically

```

## 📂 Dataset

The dataset: screentime_analysis.csv
Example columns:
⦁	**Date**: Date (dropped during preprocessing)

⦁	**App**: App name (dropped during preprocessing)

⦁	**Usage**: Time spent using the app

⦁	**Notifications**: Number of notifications received

⦁	**Times Opened**: Number of times the app was opened

Place your CSV inside data/ (e.g., data/ad_users.csv) or upload via the web UI.


## 📊 Features Used

⦁	App Usage Time

⦁	Notifications Received

⦁	App Open Count

## 🔍 Techniques Applied

⦁	Data Normalization (MinMaxScaler)

⦁	Generator & Discriminator Deep Neural Networks (DNNs)

⦁	Adversarial Training Loop (GAN)

⦁	Synthetic Data Generation

## 📌 Sample Output

Example synthetic data output (after training):

[[482.3, 18.5, 12.1],
 [397.8, 10.3, 7.6],
 [510.2, 15.8, 11.0]]

Generated to mimic real-world data distribution while ensuring privacy.

## 📈 Output

⦁	**generator.h5**: Trained Generator model

⦁	**scaler.pkl**: Saved MinMaxScaler for consistent normalization

⦁	**columns.json**: Original column names used in the dataset

## 🛠️ Tech Stack

⦁	**Backend**: Python, Google Colab

⦁	**ML/DS**: TensorFlow / Keras, Pandas, NumPy, Scikit-learn

⦁	**Utilities**: joblib (model persistence), huggingface_hub (optional model hosting)

💡 Contributions, issues, and feature requests are welcome!


---
