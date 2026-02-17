Network Intrusion Detection Using Machine Learning

📌 Project Description

This project focuses on building a Network Intrusion Detection System  using machine learning algorithms. The main objective is to detect different types of cyber attacks from network traffic data and classify them correctly.

With the rapid growth of internet usage, cyber attacks such as DoS (Denial of Service) and probing attacks have become very common. Traditional security systems sometimes fail to detect new or unknown attacks. Therefore, machine learning techniques are used in this project to automatically analyze network traffic and identify malicious activities.

---

 📊 Dataset Details

The project uses the Kyoto 2007 intrusion detection dataset, which contains real network traffic collected from honeypots and normal servers.

* Total Samples Used: 89,118
* Total Features: 24
* Data collected from: Two days of January 2007
* Each row represents one network connection record

The dataset was cleaned and preprocessed before training the models.

---

🛡 Attack Categories Identified

The network traffic was classified into the following categories:

| Code | Attack Type             | Number of Samples |
| ---- | ----------------------- | ----------------- |
| 0    | Normal Traffic          | 9,237             |
| 1    | DoS Attack              | 74,729            |
| 2    | Probe / Scanning Attack | 5,152             |
| 3    | Other Attack            | 0                 |

 Observation:

Most of the traffic in the dataset belongs to DoS attacks, which means the dataset is imbalanced. There were no samples found under the “Other Attack” category in the selected data.

---

⚙️ Tools and Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

---

 🔄 Project Workflow

The project was completed in the following steps:

1. Loaded daily text files of network logs
2. Combined multiple files into one dataset
3. Assigned proper column names
4. Cleaned and preprocessed the data
5. Encoded attack labels into numerical values
6. Split the dataset into training and testing sets (80% – 20%)
7. Trained different machine learning models
8. Evaluated performance using accuracy, ROC curve, and AUC score

---

 Machine Learning Models Used

Three different classification algorithms were implemented and compared:

 1. K-Nearest Neighbors (KNN)

Accuracy: 97.99%

 2. Random Forest

Accuracy: 99.07%

 3. Support Vector Machine (SVM)

Accuracy: 92.65%

 Best Performing Model:

The Random Forest classifier achieved the highest accuracy among all models and performed very well in detecting different attack types.

---

 📈 Model Performance

* ROC curves were plotted for evaluation.
* AUC values were close to 1.0, which indicates strong classification performance.
* The system successfully distinguishes between normal traffic and attack traffic.

---

🎯 Conclusion

This project shows that machine learning can be effectively used for detecting cyber attacks in network traffic. Among all the models tested, Random Forest provided the best results for this dataset.

The developed system can be further improved and used as a base for real-time intrusion detection applications.


