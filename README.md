# RESTTube

A microservices-based video sharing platform. This repository contains the main Docker Compose setup and includes each microservice as a git submodule.

## Getting Started

### 1. Clone the Main Repository
```sh
git clone https://github.com/Joel0423/RESTTube.git
```

### 2. Initialize and Update Submodules
```sh
git submodule update --init --recursive
```
This will fetch all microservices into their respective folders.

## Project Structure
```
RESTTube/
├── docker-compose.yml
├── RESTTube-comment-service/ (submodule)
├── RESTTube-frontend/ (submodule)
├── RESTtube-user-management-service/ (submodule)
├── RESTTube-videostream-service/ (submodule)
└── ...
```

## Usage
- Configure environment variables as needed for each service.
- Start all services with Docker Compose:
  ```sh
  docker-compose up --build
  ```

## Submodules
Each microservice is managed as a separate git repository and included here as a submodule.  
For more info on submodules, see [Git Submodules Documentation](https://git-scm.com/book/en/v2/Git-Tools-Submodules).