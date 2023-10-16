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

This dataset, comprising diverse fingerspelling gestures by both genders, is crucial for the success of our recognition system. It captures real-world signing practices, incorporating varied styles, handshapes, and gender-specific differences. Equal representation from males and females acknowledges potential articulation variations, ensuring our system accommodates diverse signing patterns. The dataset also includes variations in lighting and backgrounds, enhancing the system's robustness. This meticulously collected data forms the foundation for developing a highly accurate, inclusive, and adaptable real-time fingerspelling recognition system, addressing communication barriers for individuals with hearing impairments.

