# **Flask-K8s-App**

## **Overview**
This is a Flask application deployed on Kubernetes using Minikube and Docker.

## **Features**
- 🚀 **RESTful API** for handling requests  
- 📊 **Data visualization** using Flask and HTML templates  
- 🐳 **Containerized application** using Docker  
- ☸️ **Orchestrated deployment** on Kubernetes using Minikube  

## **Project Structure**
```plaintext
flask-k8s-app/  
│-- app.py                 # Main Flask application file  
│-- Dockerfile             # Docker configuration file  
│-- deployment.yaml        # Kubernetes deployment file  
│-- service.yaml           # Kubernetes service file  
│-- requirements.txt       # Required Python dependencies  
│-- README.md              # Documentation
```

## **Prerequisites**

Ensure you have the following installed:
- Python 
- Docker
- Kubernetes (Minikube)
- Git


## Installation

### Local Setup
1. Clone this repository:
   ```sh
   git clone https://github.com/2003DevaDharshini/flask-k8s-app.git
   cd flask-k8s-app
   
   
2.Install dependencies:
   ```sh
   pip install -r requirements.txt
```


3.Run the Flask app locally:
  ```sh
   python app.py
```

4.Docker Setup
 Build the Docker image:
 ```sh
 docker build -t flask-k8s-app
```
5.Run the container:
  ```sh
  docker run -p 5000:5000 flask-k8s-app
```
### Kubernetes Deployment
1. Start Minikube:

```sh
minikube start
```
2.Deploy the application:

```sh
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```
3.Check running pods:

```sh
kubectl get pods
```
4.Get service URL:

```sh
minikube service flask-service --url
```

### Environmental Variables
```
PORT=5000
DEBUG=True
```
