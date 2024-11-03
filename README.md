# Detection-and-Analysis-of-Audio-impairment

### (Published and Presented in conference by European Alliance for Innovation International Conference on Intelligent Systems and Machine Learning (EAI ICISML 2022))


![image](https://user-images.githubusercontent.com/71886103/199484075-4a293cfe-f87a-4e5f-b971-b716251cb3ac.png)

![image](https://user-images.githubusercontent.com/71886103/199484179-b1ba106d-fdae-419b-a3f6-10e26eb21d9e.png)

![image](https://user-images.githubusercontent.com/71886103/199484293-0c02a29c-aed8-4898-9ec5-752c2566f0bd.png)

Doctor Data Analysis Page:
![image](https://user-images.githubusercontent.com/71886103/199484906-c08b7398-e88c-491c-9c8e-ff6bc87843a7.png)

Doctor Page:
![image](https://user-images.githubusercontent.com/71886103/199484974-a8634626-a4ff-4d86-afba-11443a3fb075.png)

Upon evaluation:
Highest Accuracy Calculated: 82.5%

After predicting all test samples according to curated model:
Confusion matrix so formed:
![image](https://user-images.githubusercontent.com/71886103/199485033-dc4734fd-6fba-42e2-b57a-6178e2c40fd7.png)

R2 Score: 0.8632
MAE Score: 0.4513
EVS Score: 0.61
![image](https://user-images.githubusercontent.com/71886103/199485105-f99fc5f6-e84d-4eb2-9302-e1969d2c1edb.png)

### Abstract

Cochlear disorders are significant auditory impairments that hinder speech comprehension and affect communication and language development. This study aims to develop a web-based platform leveraging machine learning (ML) and computer vision techniques for early detection of cochlear disorders. A classification model is trained on a custom audiology dataset from the UCI machine learning repository, with cross-validation performed across multiple classification algorithms.

### Background Study

Several people worldwide face hearing impairments, with a study in Delhi reporting a 25.1% prevalence of hearing loss. Key findings include:

- **Hearing Aid Usage**: Less than 16% of adults aged 20–69 utilize necessary hearing aids, which nearly doubles to 30% for those over 70.
- **Research Techniques**: 
  - Machine Learning and Deep Learning methods for predicting hearing aid types.
  - Various classification techniques, including:
    - Logistic Regression
    - Decision Trees
    - Support Vector Classifier (SVC)
    - K-Nearest Neighbors (KNN)
    - Multi-Layer Perceptron (MLP)

### Proposed Methodology

1. **Data Preprocessing and Feature Engineering**:
   - Utilizes an audiology dataset with 70 features.
   - Normalization and outlier analysis through box plots and histograms.
   - Class imbalance addressed using RandomOverSampler, increasing samples to 1,152.

2. **Model Development**:
   - Divides the dataset into training (80%) and testing (20%).
   - Implements models: 
     - Logistic Regression
     - MLP
     - Decision Trees
     - SVM
     - KNN
   - Employs 5-fold cross-validation for robust evaluation.

3. **Face Tilt Calculation**:
   - Utilizes Haar Cascade classifiers for face and eye detection.
   - Computes tilt angle using the centers of detected eyes.

4. **Deployment**:
   - Develops a web application using Flask for user interaction.
   - Serializes the ML model using pickle for efficient deployment.

### Conclusion and Future Work

The application predicts cochlear disorders with an accuracy of 82.5% using the MLP model. Future enhancements may include dimensionality reduction techniques like Principal Component Analysis (PCA) and exploration of deep learning models to improve accuracy and efficiency.
