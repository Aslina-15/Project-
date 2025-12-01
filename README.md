Below is the merged explanation for both parts of your project:


---

PART 1 — Data Cleaning, Analysis & Visualization

1. Upload & Load Data

You upload an Excel file via Colab.

It is read into a pandas DataFrame.

You view the structure using head() and columns.



---

2. Data Cleaning

Checked for missing values using isnull().sum()

Viewed statistical info via describe()

Removed duplicate rows

Cleaned missing argsNum by replacing NaN with mean of eventId



---

3. Visualization

You generated multiple graphs including:

✔ Scatter Plots

eventId (X-axis)

argsNum (Y-axis)

Used green & red colors


✔ Pie Chart

Shows percentage share of timestamps grouped by eventId.


✔ Dashboard

Combined scatter plot + pie chart

Saved as dashboard.png



---

4. Grouping & Aggregation

Grouped by eventId

Calculated sum of timestamp

Used grouped data in pie charts



---

PART 2 — Machine Learning (TF-IDF + Naive Bayes Classifier)

1. Cleaning for ML

Removed rows without eventName (target label)

Plotted class distribution (bar chart)



---

2. Preparing Data for ML

X = all columns except eventName

y = eventName

Split into 80% train / 20% test



---

3. TF-IDF Vectorization

Since TF-IDF works on text only:

Each row is converted into one combined string

Example: "123 45 78 login success 98"

TF-IDF converts text → numerical features



---

4. Model Training (Naive Bayes)

Used Multinomial Naive Bayes classifier

Trained on TF-IDF features

Predicted test labels



---

5. Model Evaluation

✔ Accuracy

Measures performance of classifier


✔ Confusion Matrix

Shows True vs Predicted labels

Visualized with annotated color map


✔ ROC Curve (Only for 2-class dataset)

Plots TPR vs FPR

Calculates AUC score
If classes > 2 → ROC is skipped



---

FINAL SUMMARY

Your full pipeline includes:

✔ Data Cleaning

✔ Exploratory Visualizations

✔ Grouping & Aggregation

✔ ML Preprocessing

✔ TF-IDF Vectorization

✔ Naive Bayes Classification

✔ Accuracy + Confusion Matrix

✔ Conditional ROC Curve
