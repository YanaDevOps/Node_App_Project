## Description
Node_App_Project is a simple Node.js web application built using a multi-stage Docker build to optimize image size and performance. It serves as an example of creating efficient production-ready Docker images using modern techniques.

## Getting Started
### Prerequisites
- Node.js: Version 22.x or later
- Docker: Installed and configured

### Installation
 1. Clone the repository:
```bash
git clone https://github.com/YanaDevOps/Node_App_Project.git
cd Node_App_Project
```

2. Build the Docker image:
```bash
docker build -t node_app_project:1.0.0 .
```

3. Run the container:
```bash
docker run -d -p 8080:3000 --name node_app_project node_app_project:1.0.0
```

4. Open the app in your browser:
```bash
http://localhost:8080
```

## Project Structure
```
Node_App_Project/
├── Dockerfile          # Docker configuration for multi-stage builds
├── server.js           # Node.js application file
└── package.json        # Node.js dependencies and scripts
```

## Technologies Used
- Node.js 22.x
- Docker for containerization

## Features
- Multi-stage Docker build for a smaller, optimized image.
- Production environment setup (NODE_ENV=production).
- Lightweight final image using node:alpine
