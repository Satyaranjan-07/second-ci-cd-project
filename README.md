TASK-1 : Automate code deployment using ci/cd pipeline through github actions

This project uses GitHub Actions to automate the process of building, testing, and deploying a Node.js web application using Docker.

WHAT DOES THE PIPELINE DOES ?

Triggers on Push: The CI/CD pipeline runs automatically whenever code is pushed to the main branch.

Runs Tests: It installs dependencies and runs tests to ensure the code works properly.

Builds Docker Image: If tests pass, it builds a Docker image for the application.

Pushes to DockerHub: The built image is then pushed to a DockerHub repository.

Tools Used

GitHub Actions – for workflow automation

Node.js – for running the web application

Docker – for containerizing and deploying the app

DockerHub – for storing Docker images

Workflow File

The CI/CD configuration is defined in .github/workflows/main.yml.

Secrets Required

Set the following GitHub secrets in your repository under Settings → Secrets → Actions:

DOCKER_USERNAME – your DockerHub username

DOCKER_PASSWORD – your DockerHub password or access token



