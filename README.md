

# Python "Hello, World!" Dockerized Application

This project contains a simple Python application that prints "Hello, World!" and demonstrates how to containerize the app using Docker.

## Features
- Lightweight Python-based application.
- Dockerized for portability and ease of use.
- Uses a minimal Ubuntu base image.

## Prerequisites
- Install [Docker](https://www.docker.com/).

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Mnvi/Docker.git
   cd Docker
   ```

2. **Build the Docker Image**:
   ```bash
   docker build -t hello-world-app .
   ```

3. **Run the Docker Container**:
   ```bash
   docker run -p 5000:5000 hello-world-app
   ```

4. **Access the Application**:
   Visit [http://localhost:5000](http://localhost:5000) in your browser to see the output.

## Dockerfile Overview

- **Base Image**: Uses the latest Ubuntu image.
- **Dependencies**: Installs Python3 and pip.
- **Working Directory**: Sets `/app` as the workspace.
- **Environment Variable**: Default `NAME=World` for customization.
- **Command**: Executes the app with `python3 app.py`.

## What’s Next?
- Explore modifying the Python app.
- Learn about Docker Compose for multi-container apps.
- Push your image to [Docker Hub](https://hub.docker.com/) for easy sharing.
