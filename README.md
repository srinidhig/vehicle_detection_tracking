**Multi-Vehicle Detection and Tracking with Deep Learning**


**Motivation**

Multiple vehicle detection and tracking are one of the emerging hot challenging research issues in the field of intelligent transportation sectors and computer vision. Historically, this task has overcome multiple challenges such as high computational costs of development and deployment of tracking systems, lack of high-quality datasets to train models on, high error rates during prediction, and lack of extensive power and resources of sensors. With the advent of deep learning, at least the accuracy of prediction and ease of implementation have improved, making the impact of vehicle tracking more tangible. Also, with rise in number of road accidents and invention of autonomous vehicles, performing this task efficiently becomes all the more crucial. Past work in this space involved using neural networks to model associations among objects, using graph optimization algorithms, and advancements to traditional image and video processing techniques. The aim of this project is to implement a user-friendly vehicle detection and tracking system using existing datasets and machine learning algorithms, to achieve the highest possible performance in terms of predicting the vehicles themselves and their trajectories. The goal is to also design a website that can take an input video and output the same video but with bounding boxes around the moving vehicles. In phase 1 of the project, the objective is to build the most accurate vehicle detection model, that can also predict number of vehicles and in phase 2, the objective is to build the tracking mechanism with deep learning frameworks as well as deploy the system on AWS using the Flask application and use this as the backend in the final website. For this purpose, the dataset under consideration is the UA-DETRAC multi-object tracking benchmark, with over 10 hours of high-resolution traffic data, with manual annotations.


**Methodology**

Low Risk Problem: We have the video data as well as the annotations. The first step is to do exploratory analysis on the size of train, test video frames and the annotations. In particular, find frequency of different vehicle types, bounding box analysis – size and number, occlusion ratio, and weather. Then, if
necessary, some image processing techniques to reduce image dimensionality or grouping of frames. The next step is to perform vehicle detection (before tracking) using Convolutional Neural Networks, where if the input is a frame, the output is a list of bounding box dimensions that encapsulate vehicles in that frame. This can then be used to predict number of vehicles per frame. Then, using Kalman filters, provide a baseline for vehicle tracking techniques.
Date for completion: 06/23/2021

Medium Risk Problem: Improve on vehicle tracking baseline using R-CNN and YOLO deep learning methodologies, which have shown training and prediction accuracy historically. Identify best model architecture based on results on test set and gather model performance metrics from results. Create plots comparing models with different hyperparameters and save model object.
Date of completion: 07/20/2021

High Risk Problem: Deploy model on AWS using Flask application and create a webpage that uses the model in the backend. It should take an input video and locate vehicles in the video and output the same video with moving bounding boxes in real-time.
Date of completion: 08/16/2021


**Impact**

Vehicle detection and statistics in highway monitoring video scenes are of considerable significance to intelligent traffic management and control of the highway. We can use it for real-time prediction of traffic and traffic direction along with frame-wise statistics of vehicles through analysis of the output bounding boxes. Identification of causes of road accidents is imperative and recommended causes can be used to aid lawmakers enforce appropriate rules to prevent them. The system can also be employed by autonomous vehicles to detect, track, or follow other vehicles and avoid collisions. The final website can be used for traffic surveillance and vehicle monitoring.


**References**

• Extensive Collection of papers, datasets, code and other resources for object detection and tracking using deep learning – Abhineet Singh. Link: https://github.com/abhineet123/Deep-Learning-for-Tracking-and-Detection#deep_learning_

• Dataset: The UAV Project. Link: https://sites.google.com/view/grli-uavdt/%E9%A6%96%E9%A1%B5

• Boosting Multi-Vehicle Tracking with a Joint Object Detection and Viewpoint Estimation Sensor - Roberto J. López-Sastre, Carlos Herranz-Perdiguero, Ricardo Guerrero-Gómez-Olmedo, Daniel Oñoro-Rubio, Saturnino Maldonado-Bascón

• MOTS: Multi-Object Tracking and Segmentation - Paul Voigtlaender, Michael Krause, Aljosa Osep

• Vehicle Counting System using Deep Learning and Multi-Object Tracking Methods - Haoxiang Liang, Huansheng Song, Huaiyu Li, Zhe Dai

• Fast R-CNN - Ross Girshick, Microsoft Research

• You Only Look Once: Unified, Real-Time Object Detection - Joseph Redmon, Santosh Divvala, Ross Girshick, Ali Farhadi
