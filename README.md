#Automated DockerFile Generator 🐳

This project automatically generates production-ready Dockerfiles for different programming languages using AI models.
It provides two implementations:
- Local version using Ollama
- Hosted version using Google’s Gemini API

📂 #Project Structure
.
├── generate_dockerfile.py          # Local version (Ollama model)
├── generate_dockerfile_hosted.py   # Hosted version (Gemini API)
├── requirements.txt                # Python dependencies

⚙️ #Requirements
Python 3.8+
Dependencies listed in requirements.txt
Either:
Ollama installed (for local version), or
Google API key (for hosted version)
Install dependencies:
pip install -r requirements.txt

🚀 #Usage
1. Local Version (Ollama)
Run:
python generate_dockerfile.py
Enter a programming language (e.g., python, node, java) and the script will generate a Dockerfile with best practices.

2. Hosted Version (Gemini API)
Make sure you set your Google API key.
Run:
python generate_dockerfile_hosted.py
Enter a programming language, and the script will generate the Dockerfile using Google Gemini.

🧩 #Example
Enter the programming language: python
Generated Dockerfile:
FROM python:3.10-slim AS builder
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
CMD ["python", "app.py"]

🌟 #Features
-Multi-stage Dockerfile generation
-Best practices included (small base images, caching layers, etc.)
-Works with multiple programming languages
-Supports both local AI model (Ollama) and cloud model (Gemini)
