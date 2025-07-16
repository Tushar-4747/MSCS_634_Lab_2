# Lab 2: Classification Using KNN and RNN Algorithms

##  Description
This lab focuses on comparing the performance of two classification algorithms — **K-Nearest Neighbors (KNN)** and **Radius Neighbors (RNN)** — using the Wine dataset from the `sklearn` library. The dataset includes 13 features describing chemical properties of wine samples, grouped into three distinct classes. The goal is to evaluate how different values of `k` in KNN and `radius` in RNN affect classification accuracy. By visualizing these results, we aim to better understand the influence of hyperparameter tuning on model performance.

---

##  Purpose
To develop hands-on experience applying two distance-based classification algorithms (KNN and RNN) and understand:
- How hyperparameters (`k` and `radius`) influence classification outcomes.
- The challenges and trade-offs associated with each method.
- When to choose KNN vs. RNN based on dataset characteristics.

---

##  Key Insights
- **KNN Accuracy:** The classifier performed best with `k = 5`, showing a stable and high accuracy across multiple values.
- **RNN Accuracy:** Performance was highly sensitive to the `radius` parameter. Some values led to poor classification or inability to classify due to lack of neighbors.
- **Model Comparison:** KNN showed more consistent performance, while RNN required careful tuning and could struggle with sparse data regions.

---

##  Challenges Faced
- Choosing an appropriate radius for RNN was difficult. Some radius values caused errors or resulted in predictions labeled as outliers (`-1`) due to no neighbors being found.
- Normalizing data was considered but omitted, as the feature scale in the Wine dataset is reasonably balanced.
- Interpreting results where RNN failed required handling exceptions and skipping NaN values in visualizations.

---

##  Files in This Repository
- `lab2_knn_rnn.ipynb`: Jupyter Notebook with all code, visualizations, and commentary.
- `README.md`: Summary of the lab, observations, and reflections.

---


