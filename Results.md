### 📊 **Classification Report Metrics:**
Each emotion class (e.g., *angry*, *happy*) has:

- **Precision**:  
  Of all images predicted as this emotion, how many were correct?  
  > High precision = few false positives.

- **Recall**:  
  Of all actual images of this emotion, how many were correctly identified?  
  > High recall = few false negatives.

- **F1-Score**:  
  Harmonic mean of precision and recall. A balance between the two.

- **Support**:  
  Number of actual instances for that emotion in the test set.

---

### ✅ Example Interpretation (from your report):

| Emotion   | Precision | Recall | F1-Score | Support |
|-----------|-----------|--------|----------|---------|
| **happy** | 0.88      | 0.83   | 0.85     | 1825    |
- The model is **very good** at detecting "happy" faces (88% precision, 83% recall).
  
| **fear** | 0.49 | 0.51 | 0.50 | 1018 |
- Performs **poorly** for "fear" (only ~50% F1-score).

---

### 📦 **Overall Performance**:
- **Accuracy**: `0.65` → 65% of predictions were correct.
- **Macro avg**: Mean of all F1-scores (treats all classes equally).
- **Weighted avg**: Takes class imbalance into account (based on support).

---

### 🧾 Confusion Matrix:
- Shows **actual vs. predicted** counts.
- Each row: actual emotion.
- Each column: predicted emotion.
- Darker cells = more correct predictions.
  - E.g., for *happy*: 1509 correct predictions (darkest cell).
  - Misclassifications like *fear* predicted as *neutral* or *sad* can also be spotted.

---

### 🚩 Summary:
- The model performs best on **happy** and **surprise**, but struggles with **fear**, **angry**, and **disgust**.
- Overall accuracy is 65%, which is decent for emotion classification from facial expressions.

Would you like suggestions on how to improve these results?
