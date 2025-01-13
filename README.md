# Truthful vs. Deceptive Hotel Reviews Classification

## Objective
The goal of this project is to classify hotel reviews into four categories:
1. **Truthful Positive (TP)**  
2. **Truthful Negative (TN)**  
3. **Deceptive Positive (DP)**  
4. **Deceptive Negative (DN)**  

---

## Dataset
- The dataset consists of 1400 labeled reviews, evenly distributed across the four categories.
- Each review was preprocessed to ensure consistency and improve model performance.

---

## Preprocessing Steps
1. **Text Conversion**  
   All reviews were converted to lowercase for uniformity.
   
2. **Tokenization and Lemmatization**  
   Words were tokenized and reduced to their base forms using lemmatization.
   
3. **Stopword Removal**  
   Common stopwords were removed, with specific exclusions to retain relevant terms.
   
4. **Vectorization**  
   The **TF-IDF (Term Frequency-Inverse Document Frequency)** technique was used to convert text into numerical feature vectors.

---

## Models Evaluated
The following machine learning models were trained and evaluated:

1. **Linear Support Vector Classifier (SVC)**  
   - Achieved the highest accuracy: **87.86%**  
   - Utilizes hyperplanes to separate classes effectively.

2. **Gradient Boosting Classifier**  
   - Accuracy: **69.93%**  
   - Combines weak learners iteratively to improve predictions.

3. **K-Nearest Neighbors (KNN)**  
   - Accuracy: **64.29%**  
   - Struggled with high-dimensional text data due to the "curse of dimensionality."

4. **Multinomial Naive Bayes (MultinomialNB)**  
   - Accuracy: **79.29%**  
   - A probabilistic model suitable for multi-class classification.

---

## Results
- The **Linear SVC** was the top-performing model with an overall accuracy of **87.86%**.

---

## Misclassifications and Insights
- Some reviews were misclassified due to ambiguous language or exaggerations.  
- Examples of misclassifications highlighted issues with dataset labeling and model interpretation.

---

## Future Work
1. **Enhanced Preprocessing**  
   Refine handling of colloquial terms and non-standard language (e.g., "yr" to "year").
   
2. **Dataset Re-evaluation**  
   Correct mislabeled data to improve model accuracy.
   
3. **Deep Learning Models**  
   Explore advanced architectures such as RNNs, LSTMs, and Transformers for better text understanding.
   
4. **Data Augmentation**  
   Increase dataset diversity using techniques like back-translation and synonym replacement.
