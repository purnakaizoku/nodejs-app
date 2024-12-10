# nodejs-app
Better Software assignment
# Node.js CI/CD Pipeline

This repository demonstrates a CI/CD pipeline for a Node.js application using Jenkins, Docker, and Kubernetes.

## Features
- Automated testing on pull requests.
- Docker image creation and pushing.
- Kubernetes deployment.
- Slack notifications for deployment status.

## Structure
- `app.js`: Main application file.
- `test/`: Unit tests.
- `Dockerfile`: Docker image configuration.
- `k8s/`: Kubernetes deployment and service configuration.
- `Jenkinsfile`: CI/CD pipeline definition.

## Setup
1. Clone the repository:
   ```bash
   git clone <repository-url>

  # Setting Up Jenkins
Install Jenkins on your server.
Install necessary plugins:
GitHub
Docker Pipeline
Kubernetes CLI
Slack Notification
Add credentials:
Docker Hub username/password.
Kubernetes kubeconfig.
Slack credentials.
Create a new pipeline project and point it to your GitHub repository.
# Running the Pipeline
Push the project to GitHub.
Trigger the Jenkins pipeline:
Automatically on pull requests (set up a webhook).
Manually for testing.
Monitor the stages in Jenkins.
Check Slack notifications for success/failure messages.
Testing the Deployment
Verify the Kubernetes deployment:
bash
Copy code
kubectl get pods
kubectl get svc
Access the application via the LoadBalancer IP or service URL.
