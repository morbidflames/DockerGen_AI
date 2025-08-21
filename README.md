# Automated DockerFile Generator 🐋

This project automatically generates production-ready Dockerfiles for different programming languages using AI models.
It provides two implementations:
- Local version using Ollama
- Hosted version using Google’s Gemini API

## Overview

- **Automated Dockerfile Generation:**  
  Automatically generates production-ready Dockerfiles for different programming languages using AI models.  

- **Best Practices Included:**  
  Generated Dockerfiles follow Docker best practices such as small base images, installing dependencies efficiently, setting working directories, copying source code, and      multi-stage builds.  

- **Flexible Language Support:**  
  Works with multiple programming languages (e.g., Python, Node.js, Java) by simply providing the language name as input.  

- **Easy Integration:**  
  Simple command-line interface where the user enters a language, and the tool outputs a ready-to-use Dockerfile.  


## 📂 Project Structure
.  
├── generate_dockerfile.py          # Local version (Ollama model)   
├── generate_dockerfile_hosted.py   # Hosted version (Gemini API)   
├── requirements.txt                # Python dependencies

## ⚙️ Requirements
-Python 3.8+
-Dependencies listed in requirements.txt
-Either:
  *Ollama installed (for local version), or
  *Google API key (for hosted version) 
-Install dependencies:
  pip install -r requirements.txt

## 🚀 Usage
1. Local Version (Ollama)
Run:
python generate_dockerfile.py
Enter a programming language (e.g., python, node, java) and the script will generate a Dockerfile with best practices.

2. Hosted Version (Gemini API)
Make sure you set your Google API key.
Run:
python generate_dockerfile_hosted.py
Enter a programming language, and the script will generate the Dockerfile using Google Gemini.
 

## 🌟 Features
-Multi-stage Dockerfile generation  
-Best practices included (small base images, caching layers, etc.)  
-Works with multiple programming languages  
-Supports both local AI model (Ollama) and cloud model (Gemini)  

## Output
<img width="1325" height="839" alt="Screenshot 2025-08-10 164413" src="https://github.com/user-attachments/assets/407f3ddd-0f56-401e-a780-f57ba89f0f9a" />


