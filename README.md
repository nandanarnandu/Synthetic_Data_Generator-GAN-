# 🧠 Synthetic Data Generator using GANs

This project uses **Generative Adversarial Networks (GANs)** to generate synthetic app usage data that looks similar to real data. It's perfect for privacy-safe data augmentation and training machine learning models.

## 📊 What Does It Do?

- Trains a GAN on real app usage data (Usage, Notifications, Times Opened)
- Learns patterns and distributions
- Generates new, fake data that mimics the original

## 🧪 Technologies Used

- Python
- TensorFlow / Keras
- Pandas, NumPy, Scikit-learn
- Google Colab

## 📁 Dataset

We used a dataset named `Screentime-App-Details.csv`, which includes:
- `Usage` – time spent using the app
- `Notifications` – number of notifications received
- `Times opened` – number of app opens

> You can download it from [this link](https://raw.githubusercontent.com/amankharwal/Website-data/master/Screentime-App-Details.csv)

## 🛠️ How It Works

1. Preprocess data by removing date & app name columns
2. Normalize numerical columns using `MinMaxScaler`
3. Build a **Generator** model to create fake samples
4. Build a **Discriminator** to detect real vs. fake
5. Train them both using GAN training loop
6. Use the trained Generator to generate new synthetic samples
7. Rescale the generated values back to the original scale

## 📸 Sample Output

```python
[[482.3, 18.5, 12.1],
 [397.8, 10.3, 7.6],
 [510.2, 15.8, 11.0]]
