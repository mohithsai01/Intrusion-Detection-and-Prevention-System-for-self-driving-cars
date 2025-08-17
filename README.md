Intrusion Detection and Prevention System (IDPS)
📌 Overview

This project focuses on building an Intelligent Intrusion Detection and Prevention System (IDPS) tailored for self-driving vehicles and networked environments. Unlike traditional rule-based models, this system leverages deep learning techniques (CNN + Attention + RBF) to detect both known and zero-day attacks in real time, providing adaptive cybersecurity for intelligent transportation systems.

🎯 Objectives

         Develop a deep learning-based IDPS optimized for vehicular networks.
         Improve detection accuracy while reducing false positives.
         Enable real-time detection and prevention with low latency.
         Enhance public trust and safety in autonomous driving systems.

🛠 Methodology

1.Data Preprocessing
      Cleaning and handling missing values
      Normalization & standardization of features
      SMOTE / undersampling for class imbalance
      Time-window aggregation of packet features
2.Feature Extraction
       Automatic feature learning using CNNs
       Attention Mechanism to highlight critical patterns
       Radial Basis Function (RBF) for non-linear classification
       Flattening & fine-tuning for efficient computation
3.Model Architecture
       CNN layers → Feature extraction
       Attention layer → Focus on key inputs
       RBF layer → Detect subtle anomalies
       Fully connected layers → Classification (normal / intrusion)

⚙ Experimental Setup

      Hardware: Intel Core i7 (10th Gen), 16 GB RAM, 512 GB SSD
      Software: Python 3.10, TensorFlow 2.x, NumPy, Pandas, Matplotlib, Seaborn, scikit-learn
      Dataset: Vehicular telemetry & network logs (CSV format)
      Training: Federated learning setup with local client updates
      Validation: Train-test split & k-fold cross-validation

📊 Evaluation Metrics

     Accuracy = (TP + TN) / (TP + TN + FP + FN)
     Precision = TP / (TP + FP)
     Recall (Detection Rate) = TP / (TP + FN)
     F1-Score = Harmonic mean of Precision & Recall
     False Positive Rate (FPR) = FP / (FP + TN)

🚀 Results

Accuracy: 83.84%
Precision: 83.25%
Recall: 83.84%
F1-score: 83.54%
R² Score: ~0.96 (high generalization ability)

Key Insights:

     CNN + Attention + RBF outperformed traditional ML models (Decision Tree, Logistic Regression, Naïve Bayes).
     System achieved low false positives and real-time inference (few ms), making it suitable for embedded vehicular platforms.

✅ Conclusion

This project demonstrates how AI-driven IDPS can significantly enhance the cybersecurity of autonomous vehicles and IoT-based networks.
 The model balances accuracy, speed, and scalability, making it a promising solution for real-world deployment.

🔮 Future Work

Integration with real-time vehicular control systems.
Expansion to multi-vehicle (V2X) environments.
Incorporation of transformers & graph-based networks for improved detection.
Policy-driven frameworks for secure deployment.
