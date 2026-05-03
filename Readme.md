<img width="833" height="569" alt="Correlation Matrix" src="https://github.com/user-attachments/assets/2d69eb51-2dec-4bcd-935c-90f87c2d2a44" /># 📩 SMS Spam Classification using NLP & Machine Learning

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
* <a href="#project-structure">Project Structure</a>
* <a href="#how-to-run-this-project">How to Run</a>
* <a href="#author--contact">Author</a>

---

<h2 id="overview">📖 Overview</h2>

This project builds a complete **SMS Spam Detection System** using NLP techniques and machine learning models.
It processes raw text messages, transforms them into numerical features, and classifies them with high precision.

A Streamlit-based web application was developed to enable real-time SMS spam classification. The app can be executed locally.

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


```

<img width="567" height="473" alt="Spam msg Vs Ham Msg" src="https://github.com/user-attachments/assets/ad00413e-e52e-4336-ab56-4bdcd1fa0c9d" />

<img width="833" height="569" alt="Correlation Matrix" src="https://github.com/user-attachments/assets/ae0eb257-08e1-44c7-8df0-ed26ff4a033e" />


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

2. Run the app:

```bash
streamlit run app.py
```


<h2 id="author--contact">👨‍💻 Author</h2>

**Your Name**
📧 Email: anweshamondal.stat@gmail.com
🔗 LinkedIn: your-www.linkedin.com/in/anwesha-mondal-stats


---

⭐ If you found this project useful, consider giving it a star!
