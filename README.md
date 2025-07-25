# 📦 Amazon Product Reviews Analysis

This project is a comprehensive analysis of Amazon product reviews, combining **Exploratory Data Analysis (EDA)** and **Textual Sentiment Analysis** to gain insights into customer feedback, product quality perception, and sentiment distribution across different product categories.

## 📁 Project Structure

- `AmazonEDA.ipynb`: Performs general exploratory data analysis on product review datasets (including ratings, review counts, product specs).
- `Amazon_TA.ipynb`: Focuses on textual analysis, cleaning, sentiment classification, and aspect-based sentiment analysis of the reviews.

---

## 📊 Exploratory Data Analysis (`AmazonEDA.ipynb`)

### ✔️ Objectives
- Merge review data with product metadata using product names.
- Analyze the distribution of review stars per product.
- Compute statistical summaries like mean, median, and standard deviation of ratings.
- Visualize data using bar charts, dot plots, and boxplots.

### 🔍 Key Analyses
- **Review Star Summary**: Mean, std, and median ratings per product.
- **Dotplot of Ratings**: Mean ± std error bar for each product.
- **Product Frequency**: Distribution of the number of reviews per product.
- **Grouped Statistics**: Aggregated review statistics using `groupby()`.

### 📈 Visuals
- Boxplots for review star ratings by product
- Error bar plots for average ratings
- Bar charts for product frequencies

---

## 🧠 Text Analysis and Sentiment Mining (`Amazon_TA.ipynb`)

### ✔️ Objectives
- Clean and preprocess raw review text (remove stopwords, punctuation, digits, emojis, URLs).
- Perform lemmatization and normalization of repeated characters.
- Generate frequency tables and word clouds.
- Extract and analyze bigrams.
- Perform **Aspect-Based Sentiment Analysis (ABSA)** using VADER on extracted bigrams.

### 🔧 Preprocessing Steps
- Lowercasing, accent stripping
- Emoji and URL removal
- Stopword filtering
- Repeated character normalization (e.g., "greeeaaat" → "great")
- Lemmatization (via NLTK's WordNetLemmatizer)

### 📚 Corpora
Analysis was conducted on three subsets of the data:
- JBL T110BT
- JBL T205BT
- Skullcandy

### 📈 Visuals
- **Word Frequency Tables**: Top terms per product
- **Bigrams Tables**: Most common bigrams (with optional word filtering)
- **Word Clouds**: For each product corpus
- **Aspect Sentiment Charts**: Aspect terms vs. sentiment polarity (based on VADER)

---

## 📦 Dependencies

This project uses the following Python libraries:

- `pandas`
- `matplotlib`
- `seaborn`
- `nltk`
- `textblob` *(optionally used)*
- `wordcloud`
- `sklearn`
- `re`
- `collections`
- `unicodedata`
- `vaderSentiment`
- `openpyxl` or `xlsxwriter` *(for exporting to Excel)*

> Use `pip install -r requirements.txt` or manually install missing packages with `pip install <package-name>`.

---

## 📁 Output Files

- Excel summaries: Product ratings, review counts
- `.png` images: Plots and word clouds (optionally saved)
- Sentiment DataFrames per product

---

## 🚀 How to Run

1. Place the two CSV files (`specs.csv`, `reviews.csv`) in the same directory as the notebooks.
2. Open and run `AmazonEDA.ipynb` to perform exploratory analysis.
3. Open and run `Amazon_TA.ipynb` for text analysis and sentiment mining.
4. Export plots and tables as needed.

---

## 💡 Future Improvements

- Use advanced ABSA models (e.g., BERT-based transformers)
- Deploy results in a simple interactive dashboard (e.g., with `Plotly Dash` or `Streamlit`)
- Apply topic modeling (e.g., LDA) for deeper insights

---

## ✍️ Author

Developed by Angelo Capasso.  
For questions, please contact: capassoa672@gmail.com
Link of Final Dashboard: https://lookerstudio.google.com/reporting/a56ece05-9489-4051-870f-54db501a3f24/page/p_3l25x1hnud/edit 

---

