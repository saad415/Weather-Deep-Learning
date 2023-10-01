# Weather Deep Learning Image Classifier 

## Table of Contents

- [Demo](#demo)
- [Overview](#overview)
- [Motivation](#motivation)
- [Technical Aspect](#technical-aspect)
- [Installation](#installation)
- [Run](#run)
- [Deployment on Render](#deployment-on-heroku)
- [Technologies Used](#technologies-used)

## Demo

Link: https://weatherdeeplearning.onrender.com/ (Website might take 2-3 minutes to load for first time)
![Screenshot 2023-10-01 151656](https://github.com/saad415/Weather-Deep-Learning/assets/28076292/20559910-d5a2-4cfb-a277-a145fa09adaf)

## Overview

This is simple weather image classification Flask app trained on the top of pretrained VGG-16 model.This classifier can identify whether an image depicts "Cloudy," "Foggy," "Rainy," "Sunny," "Shine," or "Sunrise." 

## Motivation

The motivation behind creating this Image Classifier was to provide a user-friendly tool for real-time weather condition assessment. This classifier serves as a valuable resource for numerous applications, including weather forecasting, travel planning, and outdoor event management. Users can obtain precise weather information quickly and conveniently from images captured by cameras or sourced from various sources.

## Technical Aspect

Our Weather Image Classifier harnesses the power of deep learning and computer vision. Here's how it works:

Pretrained VGG16 Model: We utilized the VGG16 model, a well-established convolutional neural network (CNN), pretrained on a large dataset. This model serves as a feature extractor to identify crucial visual patterns within the images.

Custom Dataset Training: To enable the classifier to recognize specific weather conditions, we trained it on a custom dataset containing diverse images of different weather scenarios. This step involved fine-tuning the VGG16 model on our dataset to adapt it to the task at hand.

Flask Web Application: We developed a user-friendly web application using Flask, a Python web framework. This app allows users to upload images for weather classification.

Deployment with Docker: The Flask application is containerized using Docker for ease of deployment and scalability. We chose Render.com as our hosting platform, providing a seamless and reliable web service.

## Installation

To install the required packages and libraries, run this command in the project directory after cloning the repository:
```console
pip install -r requirements.txt
```


## Run

To run following command:
```console
python app.py
```
You'll see output indicating that the Flask development server is running. By default, the app will be available at http://localhost:5000.

## Deployment on Render

The Flask application is containerized using Docker for ease of deployment and scalability. I chose Render.com for hosting my flask application docker image.


## Technologies Used

Our Weather Image Classifier leverages a range of technologies to deliver accurate and efficient weather condition predictions:

- **Python**: The core programming language used for building the classifier and its associated components.

- **Flask**: A lightweight and powerful web framework for developing the user-friendly web application that allows users to upload images for classification.

- **Docker**: Containerization technology used for packaging the Flask application and its dependencies into a container for easy deployment and scalability.

- **VGG16 Model**: A pretrained convolutional neural network (CNN) from the Visual Geometry Group (VGG) at the University of Oxford. It serves as the backbone for feature extraction from input images.

- **Custom Dataset**: A curated dataset containing diverse weather images used for fine-tuning the VGG16 model to recognize specific weather conditions.

- **Render.com**: A cloud hosting platform utilized for deploying the Flask web application, ensuring reliable and accessible access to the Weather Image Classifier.

##
