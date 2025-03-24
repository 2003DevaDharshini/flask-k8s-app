# Flask-K8s-App

## Overview
This is a Flask application deployed on Kubernetes using Minikube and Docker.

## Features
- Feature 1
- Feature 2
- Feature 3

## Project Structure
flask-k8s-app/
│-- app.py
│-- Dockerfile
│-- deployment.yaml
│-- service.yaml
│-- README.md
## Prerequisites
- Python 3.x
- Docker
- Kubernetes (Minikube)
- Git
- Any required dependencies

## Installation
### Local Setup
Clone this repository:
git clone https://github.com/2003DevaDharshini/flask-k8s-app.git
cd flask-k8s-app

## Install dependencies:
pip install -r requirements.txt

Run the Flask app locally:
python app.py

### Docker Setup
Build the Docker image:
docker build -t flask-k8s-app

Run the container:
docker run -p 5000:5000 flask-k8s-app

###Kubernetes Deployment
Start Minikube:
minikube start

Deploy the application:
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

Check running pods:
kubectl get pods

Get service URL:
minikube service flask-service --url

Environmental Variables
The following environment variables can be configured:
PORT=5000
DEBUG=True