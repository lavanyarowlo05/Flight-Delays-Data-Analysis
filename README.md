# Flight Delay Predictor

## Project Overview

The Flight Delay Predictor is a machine learning project designed to predict whether a flight will be delayed based on historical flight data. A flight is considered delayed if it arrives 15 minutes or more late, according to the Federal Aviation Administration (FAA) standards.

This project builds an end-to-end machine learning pipeline that analyzes historical flight information to identify delay patterns and predict future flight delays. The goal is to help airlines improve operational planning and reduce the impact of delays on passengers and airline operations.

## Business Problem

Flight delays create several challenges for airlines:

Reduced customer satisfaction

Increased operational costs

Scheduling disruptions across flight networks

Predicting flight delays in advance can help airlines optimize scheduling, improve resource allocation, and enhance overall operational efficiency.

## Objective

The objective of this project is to build a robust machine learning pipeline for predicting flight delays while incorporating key MLOps practices such as:

Experiment tracking

Workflow orchestration

Model deployment

Model monitoring

Reproducible environments

The system ensures that the model only uses features available at prediction time to avoid data leakage, making the model reliable for real-world use.

## Dataset

The dataset used in this project comes from the Bureau of Transportation Statistics – Reporting Carrier On-Time Performance dataset.

The dataset includes:

Arrival information (arrival times and delays)

Departure information (departure times and delays)

Origin airport details

Destination airport details

Airline carrier information

Flight scheduling data

Key features used for training include:

Day of Month

Day of Week

Airline

Origin Airport

Destination Airport

Scheduled Departure Time

Scheduled Arrival Time

Scheduled Elapsed Time

## Technologies Used

Python
Scikit-learn
XGBoost
MLflow
Prefect
Evidently
Docker
AWS S3

These tools help build a complete production-ready machine learning pipeline.

## Machine Learning Pipeline

The project includes the following components:

Experiment Tracking

MLflow is used to track model experiments, log parameters, and compare model performance.

Workflow Orchestration

Prefect manages and schedules the machine learning pipeline tasks.

Model Deployment

The trained model is deployed using Docker and exposed through an API endpoint that predicts flight delays.

Model Monitoring

Evidently monitors model performance and detects potential data drift.
