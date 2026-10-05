# 🤖 AI-Based Product Recommendation Chatbot Using Machine Learning

## 📌 Project Overview

The **AI-Based Product Recommendation Chatbot** is a machine learning project developed using **Python and Google Colab**.

The system recommends suitable products based on the user's requirements. It understands the product category and budget mentioned in the user's query and uses **TF-IDF vectorization** and **Cosine Similarity** to find products that are most relevant to the user's needs.

This project uses a **content-based recommendation approach** and does not require an external website or large language model.

---

## 🎯 Objectives

* Recommend products based on user requirements.
* Identify the product category from a natural-language query.
* Detect the user's maximum budget.
* Rank products based on textual similarity.
* Provide an interactive chatbot experience.
* Store recommendation history.
* Analyze recommendation results.
* Visualize recommendation data.

---

## 🛠️ Technologies Used

| Technology        | Purpose                        |
| ----------------- | ------------------------------ |
| Python            | Main programming language      |
| Google Colab      | Development environment        |
| Pandas            | Data handling and analysis     |
| NumPy             | Numerical operations           |
| Scikit-learn      | Machine learning and NLP       |
| Matplotlib        | Data visualization             |
| Seaborn           | Visualization                  |
| TF-IDF            | Text feature extraction        |
| Cosine Similarity | Product similarity calculation |

---

## 🧠 Machine Learning Technique

### Content-Based Filtering

The system uses **content-based filtering**.

Products are recommended by comparing the user's query with product information such as:

* Product name
* Category
* Brand
* Description

The system calculates how similar the user's query is to each product.

### TF-IDF

**TF-IDF (Term Frequency-Inverse Document Frequency)** converts product text into numerical vectors.

### Cosine Similarity

Cosine Similarity measures the similarity between the user's query vector and the product vectors.

Products with higher similarity scores are ranked higher in the recommendations.

---

## 📊 Dataset

The project uses a **sample product dataset created directly in Python** for demonstration and machine learning purposes.

The dataset contains **20 products** from the following categories:

* 💻 Laptop
* 📱 Smartphone
* 🎧 Headphones
* 📱 Tablet
* 📷 Camera

### Dataset Columns

```text
product_id
product_name
category
brand
price
rating
description
```

The prices in this dataset are **sample values for the project** and should not be treated as current market prices.

---

## ⚙️ How the System Works

```text
User Query
     ↓
Text Cleaning
     ↓
Category Detection
     ↓
Budget Detection
     ↓
TF-IDF Vectorization
     ↓
Cosine Similarity
     ↓
Category & Price Filtering
     ↓
Similarity Ranking
     ↓
Top Product Recommendations
     ↓
Recommendation History
```

---

## 🔍 Main Features

### 1. Product Recommendation

The chatbot accepts natural-language product requirements.

Example:

```text
I need a laptop for programming
```

The system identifies relevant products and recommends the most similar ones.

---

### 2. Category Detection

The chatbot detects categories such as:

```text
Laptop
Smartphone
Headphones
Tablet
Camera
```

It also recognizes related words such as:

```text
computer → Laptop
mobile → Smartphone
earbuds → Headphones
tab → Tablet
DSLR → Camera
```

---

### 3. Budget Detection

The chatbot can identify budget requirements from queries.

Examples:

```text
laptop under 60000
phone below 30000
headphones within 7000
tablet up to 35000
```

The system then filters products according to the specified budget.

---

### 4. Smart Recommendation

The system combines:

* Category detection
* Budget filtering
* TF-IDF
* Cosine Similarity
* Similarity ranking

to produce more relevant recommendations.

---

### 5. Interactive Chatbot

Users can interact with the chatbot directly in Google Colab.

Example:

```text
👤 You: I need a laptop for programming under 60000

🤖 Chatbot: Here are some products I recommend for you!
```

The chatbot continues accepting queries until the user enters:

```text
exit
```

---

### 6. Recommendation History

The system stores previous recommendations including:

* User query
* Product name
* Category
* Brand
* Price
* Rating
* Similarity score

This allows recommendation results to be analyzed later.

---

### 7. Data Analysis

The project calculates:

* Total recommendations
* Most recommended categories
* Average product price
* Average product rating
* Average similarity score

---

### 8. Data Visualization

The project visualizes recommendation results using:

* Matplotlib
* Seaborn

For example, a category-wise recommendation chart is generated.

---

## 📁 Project Structure

```text
Product_Recommendation_Chatbot/
│
├── Product_Recommendation_Chatbot.ipynb
├── product_dataset.csv
├── product_tfidf_vectorizer.pkl
└── README.md
```

### File Description

**Product_Recommendation_Chatbot.ipynb**

Contains the complete project code, including data preparation, machine learning, chatbot implementation, testing, analysis, and visualization.

**product_dataset.csv**

Contains the sample product dataset.

**product_tfidf_vectorizer.pkl**

Contains the trained TF-IDF vectorizer saved using Python Pickle.

**README.md**

Contains the project documentation.

---

## 🚀 How to Run the Project

### Step 1: Open Google Colab

Upload:

```text
Product_Recommendation_Chatbot.ipynb
```

### Step 2: Run the notebook cells

Run the cells from top to bottom.

### Step 3: Install the required libraries

The notebook installs:

```text
pandas
numpy
scikit-learn
matplotlib
seaborn
```

### Step 4: Run the chatbot

After running all required cells, enter product requirements such as:

```text
I need a laptop for programming under 60000
```

or:

```text
Suggest a phone for gaming under 30000
```

---

## 🧪 Example Queries

```text
I need a laptop for programming under 60000
```

```text
Suggest a smartphone for gaming under 30000
```

```text
I need headphones for music under 7000
```

```text
Suggest a tablet for studying under 35000
```

```text
I want a camera for photography under 70000
```

---

## 🔮 Future Enhancements

The project can be further improved by adding:

* Larger real-world product datasets
* More product categories
* Advanced natural-language processing
* User preference learning
* Collaborative filtering
* Product availability checking
* Real-time product prices
* Product reviews and sentiment analysis
* Web or mobile interface
* Voice-based interaction
* Deployment as an online application

---

## 📌 Limitations

* The current dataset contains only 20 sample products.
* Product prices are sample values.
* Recommendations depend on the available product descriptions.
* The chatbot uses rule-based category and budget detection.
* It does not retrieve live product information from online stores.

---

## 🎓 Project Type

**Domain:** Artificial Intelligence & Machine Learning

**Project Type:** Machine Learning / NLP / Recommendation System

**Platform:** Google Colab

**Language:** Python

**Recommendation Method:** Content-Based Filtering

---

## 👩‍💻 Author

**Jaya Shree S**

B.E. Computer Science and Engineering

Prathyusha Engineering College
