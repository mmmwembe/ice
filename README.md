# Flask App with Docker

This is a Flask application designed to run locally and in a Docker container. Follow the instructions below to build, run, and access the application.

---

## Prerequisites

Ensure you have the following installed:
- [Docker](https://www.docker.com/)
- Python (optional, for local development)

---

## Running the Flask App Locally with Docker

```bash
# 1. Build the Docker image
docker build -t app .

# 2. Run the Docker container
docker run -p 8080:8080 app

# If your app uses environment variables (e.g., .env file), run with:
docker run --env-file .env -p 8080:8080 app

# 3. Access the app in your browser
# Open http://localhost:8080

# Cleanup unused containers
docker system prune

# Run code locally
python app.py


