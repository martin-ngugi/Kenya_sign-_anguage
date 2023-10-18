
# Real-Time Sign Language Hand Detection

![ksl image](https://github.com/BetshuaK/The_Black_Tide/raw/main/ksl%20image.png?raw=true)

Collaborators: [Kimberly Wairimu](https://github.com/KimberlyWairimu), [Martin Ngugi](https://github.com/martin-ngugi), [Raphael Muthemba](https://github.com/Rafael-Muthemba), [Bonventure Osoro](https://github.com/osoroSan), [Joseph Mwaniki](https://github.com/JosephMwaniki), [Betshua Kerubo](https://github.com/BetshuaK)

## Table of Contents

* Business Understanding
* Data Understanding
* Data Preparation
* Modeling
* Evaluation

## 1.Business Understanding

### Introduction

In a world where effective communication is fundamental, individuals with disabilities, particularly those relying on sign language, face significant challenges. Finger spelling, a crucial aspect of communication for the Deaf and Hard of Hearing, bridges this gap. Yet, there's a blunt communication division leading to social seclusion and limited opportunities. Recognizing this, the Ministry of Public Services, Gender, Senior Citizens Affairs, and the special Program and Rehabilitative Services Division has embarked on a transformative initiative to break down the barriers faced by individuals with this kind of disability. Our project will harness the power of advanced computer vision techniques to detect and interpret the intricate handshapes and movements that constitute fingerspelling. This will aim to empower individuals and enhance communication. By breaking barriers, we improve the Ministry's ability to serve citizens with disabilities, fostering inclusivity and accessibility in essential services.

### Problem Statement

Effective communication is a fundamental human right and an essential component of social inclusion and participation. However individuals with hearing impairments who rely on fingerspelling as their primary means of communication face often significant communication barriers.The problem at hand is limited accessibility and inclusivity faced by individuals with hearing impairments who rely on fingerspelling.Current communication solutions do not adequately facilitate effective communication between individuals proficient in this visual-gesture language. The Ministry of Public Services,Gender, Senior Citizens Affairs and Special Program and Rehabilitative Services Division have commissioned this project to develop and implement a real-time fingerspelling detection system that can bridge the communication gap between individuals with hearing impairments to communicate effectively with the government officials,access government services, education, and employment opportunities and promote their overall social inclusion and well-being.

### Metric of Success

* Recognition Accuracy

Achieve a recognition accuracy rate of at least 90%, measured by the percentage of correctly identified fingerspelled words out of the total fingerspelled words processed by the system.

 * Response Time

Ensure a response time of less than 20 seconds for recognizing and translating fingerspelling gestures into text or speech in real time.

* Error Rate

Maintaing a low error rate, with recognition errors accounting for less than 5% of total interactions with the system.

* Integration Success
  
Integrate the system succesfully into a website, ensuring seamless functionality.

### Objectives

#### Main Objective: 

* To develop and implement a real-time fingerspelling detection system that empowers individuals with hearing impairments to communicate effectively with the broader community,government officials and service providers,thereby promoting inclusivity,accessibility and social intergration.

#### Specific Objectives:

* Data Collection

Collect a diverse and comprehensive dataset of fingerspelling gestures performed by individuals with varying signing styles,hand shapes and speeds

* Develop a robust hand detection system

Create an accurate and robust hand detection system using cvzone and MediaPipe to ensure precise tracking of hand movements during fingerspelling.

* Implement fingerspelling recognition

Develop a recogntion component that can identify and interpret fingerspelled words and gestures in real-time using machine learning algorithms.

* Real-time translation

Intergrate a translation mechanism that converts detected fingerspelled letters into text in real-time,ensuring immediate and accessible communication.

* User-Friendly Interface

Design an intuitive user interface that is accessible and user-friendly, allowing individuals with disabilities to interact with the system comfortably

* Intergration into a website

Develop a website to intergrate the system to maximize its reach and impact.

## 2. Data Understanding

The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/datamunge/sign-language-mnist)

**Content**: The dataset features grayscale images (28x28 pixels) of hand signs representing the American Sign Language (ASL) alphabet, excluding J and Z due to hand motion. Pixel values range from 0 to 255, where 0 is black and 255 is white, representing different shades of gray. The images effectively capture the shape and orientation of hand gestures corresponding to letters A-Z in ASL.

**Format**: The dataset format closely matches the classic MNIST dataset. It includes a header row of the label and pixel values of pixel1 to pixel784.

**Size**: The dataset contains 27,455 cases for training and 7,172 cases for testing.

To enhance diversity and volume, group members contributed extra images. Notably, there's no significant difference between fingerspelling in ASL and Kenyan Sign Language (KSL), allowing interchangeability.

## 3. Data Preparation

Within our data preparation phase, we performed the following tasks:

* Clean Data
* Data Wrangling
* Image processing
* Feature Engineering

### EDA

The following analysis was performed on the data:

* Displaying the images along with their labels.
* Visualizing the frequency distribution of labels in both the train and test datasets.
* Pixel distribution

## 4. Modeling

The models include;

* Dense neural network
* Convolution neural network

## 5. Evaluation

Our success metrics is accuracy. The model that had the highest accuracy for the validation set was chosen to be the best model and thus used to predict the fingerspelling images.

## 6. Conclusions

1. Pixel distribution suggests important features in the center, impacting model learning.

2. Baseline and Second Models show signs of overfitting, with high training accuracy and lower validation accuracy.

3. First and Third Models perform better, demonstrating effective learning and generalization.

4. Model complexity aligns with performance, with the Third Model being the most complex.

5. Dropout layers help prevent overfitting, but additional regularization may be needed due to persisting issues in some models.

## 7. Recommendations

1. For models showing overfitting (Baseline and Second Model), consider regularization techniques like dropout or early stopping. Increasing training data may also help reduce overfitting.

2. Monitor the performance of high-performing models (First and Third Model) on new unseen data to ensure sustained effectiveness over time.

3. If image features are concentrated in the center, explore preprocessing techniques like center-cropping or attention mechanisms to enhance model performance by reducing noise.

4. The Third Model, with a training accuracy of 99.48% and test accuracy of approximately 94.62%, seems to be the best choice. It incorporates various techniques to prevent overfitting and demonstrates effective learning and generalization.

## 8. Next Steps

1. Evaluate the models on a regular basis using new, unseen data to ensure they continue to perform well and can generalize to new data.

2. Setting up a system for monitoring model performance over time. This will allow you to quickly identify and address any issues that may arise.

3. Consider using pretrained models which have been trained on large datasets and have proven success in image classification tasks. These models can be fine-tuned on your specific task and often provide a good starting point.

