
# Docker CI Learning Project

![Python](https://img.shields.io/badge/Python-3.13-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Framework-green)
![Docker](https://img.shields.io/badge/Docker-Container-blue)
![Status](https://img.shields.io/badge/Status-Active-success)

## About

A learning project built using Python, FastAPI and Docker.
This project demonstrates how to create and run a FastAPI application
and package it using Docker.

## Technologies Used

- Python
- FastAPI
- Uvicorn
- Docker
- Pytest
- Git and GitHub

## Project Structure

```text
my-docker-app/
│
├── tests/
├── .dockerignore
├── .gitignore
├── Dockerfile
├── main.py
├── requirements.txt
└── README.md
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | / | Home |
| GET | /about | About |
| GET | /health | Health Check |
| GET | /products | Get Products |

## How to Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/KajalHonde/docker-ci-learning-project.git
cd docker-ci-learning-project
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the environment (Windows CMD)

```cmd
.venv\Scripts\activate.bat
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Start the application

```bash
uvicorn main:app --reload
```

### 6. Open API documentation

http://127.0.0.1:8000/docs

## Run Using Docker

### Build Docker Image

```bash
docker build -t my-docker-app .
```

### Run Docker Container

```bash
docker run -p 8000:8000 my-docker-app
```

Open:

http://127.0.0.1:8000/docs

## Testing

Run tests using:

```bash
pytest
```

## Author

Kajal Honde
