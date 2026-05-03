# 📩 SMS Spam Classification using NLP & Machine Learning

*An end-to-end Natural Language Processing (NLP) project to classify SMS messages as Spam or Ham using machine learning, with deployment as an interactive web application.*

---

## 📌 Table of Contents

* <a href="#overview">Overview</a>
* <a href="#business-problem">Business Problem</a>
* <a href="#dataset">Dataset</a>
* <a href="#tools--technologies">Tools & Technologies</a>
* <a href="#project-workflow">Project Workflow</a>
* <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
* <a href="#model-building">Model Building</a>
* <a href="#model-performance">Model Performance</a>
* <a href="#web-application">Web Application</a>
* <a href="#deployment">Deployment</a>
* <a href="#project-structure">Project Structure</a>
* <a href="#how-to-run-this-project">How to Run</a>
* <a href="#future-improvements">Future Improvements</a>
* <a href="#author--contact">Author</a>

---

<h2 id="overview">📖 Overview</h2>

This project builds a complete **SMS Spam Detection System** using NLP techniques and machine learning models.
It processes raw text messages, transforms them into numerical features, and classifies them with high precision.

The final solution is deployed as a **Streamlit web app**, allowing real-time predictions.

---

<h2 id="business-problem">💼 Business Problem</h2>

Spam messages are a major issue for communication platforms. The goal is to:

* Automatically detect spam messages
* Minimize false positives (important messages marked as spam)
* Build a scalable and efficient classification system

---

<h2 id="dataset">📂 Dataset</h2>

* Source: **Kaggle SMS Spam Dataset**
* Target Variable:

  * **Spam → 1**
  * **Ham → 0**

---

<h2 id="tools--technologies">🛠️ Tools & Technologies</h2>

* **Programming:** Python
* **Libraries:**

  * Pandas, NumPy
  * NLTK
  * Scikit-learn
  * Matplotlib, Seaborn
* **Modeling:** Naive Bayes, Tree-based models, Ensemble models
* **Deployment:** Streamlit, Render

---

<h2 id="project-workflow">⚙️ Project Workflow</h2>

## 🔍 Project Workflow

### 1️⃣ Data Cleaning

* Removed unwanted columns
* Renamed columns for clarity
* Label encoding:

  * Spam → 1
  * Ham → 0
* Checked for null values
* Removed duplicate records

---

### 2️⃣ Exploratory Data Analysis (EDA)

* Distribution of Spam vs Ham messages (Pie Chart)
* Observed slight class imbalance
* Created features:

  * Number of characters
  * Number of words
* Compared Spam vs Ham using histograms
* Correlation heatmap

📊 **EDA Visualizations:**
(Add your images here)

```
![EDA 1](path/to/image)
![EDA 2](path/to/image)
```

---

### 3️⃣ Text Preprocessing

Steps performed:

* Lowercasing
* Tokenization
* Removing stopwords & punctuation
* Stemming (Porter Stemmer)

Custom function used:

```
transform_text()
```

---

### ☁️ WordCloud Visualization

* WordCloud for Spam messages
* WordCloud for Ham messages

(Add images here)

```
![Spam WordCloud](path/to/image)
![Ham WordCloud](path/to/image)
```

---
---

<h2 id="model-building">🤖 Model Building</h2>

### Vectorization Techniques

* Count Vectorizer
* **TF-IDF Vectorizer (Best Performance)**

### Models Tested

* Gaussian Naive Bayes
* Multinomial Naive Bayes
* Bernoulli Naive Bayes
* Decision Tree
* KNN
* Random Forest
* AdaBoost
* Bagging
* Extra Trees
* Gradient Boosting
* XGBoost

📌 **Best Model Selected:**

* **Multinomial Naive Bayes + TF-IDF**

---

<h2 id="model-performance">📈 Model Performance</h2>

| Metric    | Value |
| --------- | ----- |
| Accuracy  | 0.978 |
| Precision | 1.00  |

📌 Precision is prioritized to ensure spam detection is highly reliable.

---

<h2 id="web-application">🌐 Web Application</h2>

* Built using **Streamlit**
* User inputs SMS text
* System performs:

  1. Text preprocessing
  2. Vectorization
  3. Prediction

### Output:

* **Spam** or **Not Spam**

---

<h2 id="deployment">🚀 Deployment</h2>

* Deployed on **Render**

👉 Add your live link here:

```
https://your-app-link.onrender.com
```

---

<h2 id="project-structure">📁 Project Structure</h2>

```
sms-spam-classifier/
│
├── data/
├── notebooks/
├── model.pkl
├── vectorizer.pkl
├── app.py
├── README.md
```

---

<h2 id="how-to-run-this-project">▶️ How to Run This Project</h2>

1. Clone the repository:

```bash
git clone https://github.com/your-username/sms-spam-classifier.git
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the app:

```bash
streamlit run app.py
```


<h2 id="author--contact">👨‍💻 Author</h2>

**Your Name**
📧 Email: [your-email@gmail.com](mailto:your-email@gmail.com)
🔗 LinkedIn: your-link
🔗 GitHub: your-link

---

⭐ If you found this project useful, consider giving it a star!
