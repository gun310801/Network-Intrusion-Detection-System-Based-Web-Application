# Network Intrusion Detection System Based Web Application

## Overview

This project implements a Network Intrusion Detection System (IDS) using machine learning and a Flask web application. The IDS analyzes network traffic for suspicious activity and classifies it into different attack categories. The web application provides a user interface to input network features and receive real-time intrusion predictions.

## Project Structure

The project consists of the following main components:

-   **Data Preprocessing:** Cleans and prepares the NSL-KDD dataset for training the machine learning models.
-   **Feature Selection:** Employs feature selection techniques like SelectKBest to identify the most relevant features for intrusion detection.
-   **Machine Learning Models:** Implements and evaluates various machine learning classifiers, including Logistic Regression, Decision Trees, K-Nearest Neighbors, and Neural Networks.
-   **Flask Web Application:** Creates a web interface for users to interact with the IDS, input network features, and receive intrusion predictions.
-   **Model Deployment:** Integrates the trained machine learning model into the Flask web application for real-time predictions.

## Introduction

Intrusion detection is a critical aspect of network security. This project aims to develop a robust and effective IDS that can identify known vulnerabilities and detect new, unknown potential device abuses. The system audits network traffic for suspicious activity and generates alerts when malicious activity is discovered.

## Features

*   **Real-time Intrusion Detection:** Classifies network packets in real-time based on collected network flow data.
*   **Machine Learning Classifiers:** Utilizes various machine learning classifiers to increase the accuracy of intrusion detection.
*   **Feature Selection:** Employs SelectKBest technique for optimal feature selection.
*   **Web Application Interface:** Provides a user-friendly web interface for easy interaction and prediction input.
*   **Attack Category Classification:** Identifies and classifies network intrusions into specific attack classes (DOS, PROBE, R2L, U2R).
*   **Low False Positive Rate:** Designed to minimize false positives and reduce false alarms.

## Dataset

The project uses the NSL-KDD dataset, a refined version of the KDD 99 dataset. The NSL-KDD dataset addresses some of the issues in the original KDD 99 dataset, such as redundant and duplicate records.

*   **Features:** Each record in the dataset consists of 43 attributes representing various features of network packets.
*   **Labels:** Each packet is labeled as either normal or one of the four attack categories: DOS, PROBE, R2L, and U2R.

### Attack Categories

*   **DOS (Denial of Service):** Attacks that make a system or network unavailable to legitimate users.
*   **U2R (User to Root):** Attacks where an attacker gains root or administrator privileges on the system.
*   **Probe:** Attacks where an attacker gathers information about the network or system.
*   **R2L (Remote to Local):** Attacks where an attacker gains unauthorized access to the system from a remote location.

## Algorithms

The following machine learning algorithms were implemented and evaluated:

*   Decision Tree Classifier
*   Logistic Regression (Selected as the best model)
*   K-Nearest Neighbors
*   Linear Discriminant Analysis
*   Bernoulli Naive Bayes
*   Gaussian Naive Bayes
*   Support Vector Machine
*   Stochastic Gradient Descent
*   Neural Network
*   Random Forest
*   Extra Trees
*   AdaBoost
*   Stochastic Gradient Boosting

## Results

The Logistic Regression model achieved the highest accuracy of 93.2% on the NSL-KDD dataset. Other models also showed promising results, but Logistic Regression was selected for its superior performance.
