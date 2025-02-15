# Sentiment Analysis of Productivity Apps 📊🤖

This project performs **sentiment analysis** on user reviews of popular productivity apps available on the Google Play Store. The goal is to classify reviews into **positive**, **neutral**, or **negative** sentiments using a **BERT-based model**. 🧠💡

---

## Table of Contents 📑
1. [Overview](#overview-)
2. [Installation](#installation-)
3. [Usage](#usage-)
4. [Code Structure](#code-structure-)
5. [Results](#results-)
6. [License](#license-)

---

## Overview 🚀

This project:
- Scrapes app reviews from the Google Play Store using the `google-play-scraper` library. 🕸️📥
- Preprocesses the data and performs sentiment analysis using a **BERT model** from the `transformers` library. 🤖📊
- Trains and evaluates the model to classify reviews into **positive**, **neutral**, or **negative** sentiments. 🎯📈
- Visualizes the results using **confusion matrices** and **bar plots**. 📊📉

---

## Installation 🛠️

To run this project, you need to install the required libraries. Run the following commands:

```bash
!pip install google-play-scraper
!pip install transformers
!pip install torch
!pip install seaborn matplotlib
!pip install pandas tqdm
```

---

## Usage 🖥️

1. **Scrape App Reviews**: The script scrapes reviews for a list of productivity apps from the Google Play Store.
2. **Preprocess Data**: The reviews are preprocessed and labeled based on their sentiment (positive, neutral, negative).
3. **Train BERT Model**: A BERT-based sentiment classifier is trained on the labeled data.
4. **Evaluate Model**: The model's performance is evaluated using accuracy, confusion matrices, and classification reports.
5. **Predict Sentiment**: The trained model can predict the sentiment of raw text inputs.

---

## Code Structure 🗂️

- **Data Collection**:
  - Scrapes app information and reviews using `google-play-scraper`.
  - Stores the data in CSV files (`app_infos.csv` and `app_reviews.csv`).

- **Sentiment Analysis**:
  - Uses a pre-trained BERT model (`bert-base-cased`) for sentiment classification.
  - Splits the data into training, validation, and test sets.
  - Trains the model using PyTorch and evaluates its performance.

- **Visualization**:
  - Plots token length distributions.
  - Displays confusion matrices and sentiment probability bar plots.

---

## Results 📊

- **Model Accuracy**: The model achieves an accuracy of **X%** on the test set.
- **Confusion Matrix**: Visualizes the model's performance across sentiment classes.
- **Sentiment Prediction**: The model can predict the sentiment of raw text inputs with high confidence.

---

## License 📜

This project is licensed under the **MIT License**. Feel free to use, modify, and distribute it as needed.

---

## Example Output 🖼️

Here’s an example of the model predicting the sentiment of a review:

```plaintext
Review text: I hated this movie. The acting sucked. The dialogue was slow.
Sentiment  : Negative
```

---

## Dependencies 📦

- `google-play-scraper`
- `transformers`
- `torch`
- `pandas`
- `seaborn`
- `matplotlib`
- `tqdm`

---

## Author 👨‍💻

This project was created by **[Navid Falah](https://github.com/navidfalah)**. Feel free to reach out for questions or collaborations at **navid.falah7@gmail.com**! 🤝
