# Cow-Emotions-and-Posture-Analysis-

### Emotion Detection in Cows using Machine Learning

This repository contains a machine learning pipeline designed to detect the emotions of cows based on their poses. The aim is to identify whether a cow is happy or unhappy by analyzing their body poses in images. The project primarily uses two deep learning models to achieve this: one for identifying cow poses and another for recognizing their emotions.

#### Project Overview
The project workflow is structured into three main stages: data preprocessing, training, and evaluation.

#### Project Flow Structure
The project involves the use of two distinct models to identify cow emotions. The workflow encompasses various steps commonly used in building deep learning models.

##### Step 1: Pose Estimation
The initial step involves employing the DEEPLABCUT Python library to identify the poses of cows in images. This library, known for estimating animal poses, simplifies both model building and data processing. The annotation process involves marking 16 key landmarks on the cow.

##### Step 1.1: Data Preprocessing
Data preprocessing involves labeling the key points on the cow's body parts and creating essential files for training the model.

##### Step 1.2: Model Training
The DEEPLABCUT pose estimation model, built on the RESNET architecture, is trained on a specific number of iterations and parameters to achieve optimal performance.

##### Step 1.3: Model Prediction
The trained model is used to predict cow poses on test images. The predictions are saved in a CSV file for further analysis and evaluation.

##### Step 2: Emotion Recognition
The next step involves the utilization of a Simple Recurrent Neural Network (RNN) model to recognize cow emotions based on the coordinates obtained in the previous step. The RNN model is trained using labeled data and is subsequently used to predict cow emotions.

##### Step 2.1: Coordinates Preprocessing
The coordinates obtained from pose predictions are structured and prepared for input into the RNN model for emotion recognition.

##### Step 2.2: Emotion Prediction
The trained RNN model is used to predict cow emotions based on the processed coordinates.

#### Project Pipeline
The implemented models allow the creation of an automated pipeline to predict cow emotions through keypoints. This pipeline offers scalability and can be used for single or multiple images.

#### Future Work
The project has potential for further enhancement, such as increasing training iterations for improved results and scalability. Additionally, scaling the project for video frame analysis is a possibility for future development.

### How to Use

To utilize the project functionalities, follow the methods outlined in the repository.

For detailed implementation and utilization, refer to the provided code and documentation in the repository.

#### Disclaimer
This project is a demonstration and should be used with caution. Results may vary and additional fine-tuning or adaptations may be required for different contexts or scenarios.

#### Future Developments
Ongoing efforts to enhance the model's accuracy and scalability are planned. New features and improvements will be updated in the repository.

### Acknowledgments
We acknowledge the contributions of the DEEPLABCUT library and the underlying deep learning models utilized in this project.

### Output Results
<img src="WhatsApp Image 2022-12-01 at 1.15.32 AM (1).jpeg" /> <br>
<img src="WhatsApp Image 2022-12-01 at 1.15.31 AM.jpeg" /> <br>

