# Deploy_SSH
This repository contains a simple project along with a deployment script for automatic deployment on a remote server using SSH key-based authentication. The deployment is done directly from this repository using a optionally via GitHub Actions.

# SSH Deployment with GitHub Actions
This repository shows how to deploy files to a remote server using SSH and GitHub Actions.

# Files Included
Saludo_Kevin.txt: Greeting file uploaded to the server to confirm successful deployment.
.github/workflows/deploy.yml: GitHub Actions workflow to automate the deployment.
How It Works
Secrets are added in GitHub Actions:

SSH_PRIVATE_KEY
SSH_HOST
USER_NAME
PROJECT_PATH
GIT_REPO
When code is pushed to the main branch:

GitHub Actions connects to the server using SSH.
The server pulls the latest version of the project.
Manual SSH Access
You can also connect manually to check:

ssh -i pemSMacServerEstudiantes ndgserver@201.190.115.29