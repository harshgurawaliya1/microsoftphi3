﻿# Image Analysis and Question Generation App

This repository contains a Flask web application that uses the Microsoft Phi-3 Vision-128k-Instruct model to analyze images and generate insightful questions based on their content. The app allows users to upload images and receive detailed, AI-generated responses about the image.

## Features

- Upload images via a simple web interface or API
- Analyze images using the state-of-the-art Phi-3 Vision-128k-Instruct model
- Generate detailed questions and responses based on image content
- Easy-to-use Flask web application

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/harshgurawaliya1/image-analysis-question-generation.git
    cd image-analysis-question-generation
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Running the Application

1. Start the Flask application:
    ```bash
    python app.py
    ```

2. The application will run on `http://0.0.0.0:5000`. You can use an API client like Postman or curl to interact with the app.

### Usage

- **API Endpoint**: `/analyze`
  - **Method**: POST
  - **Form Data**: `image` (file)
  - **Response**: JSON containing the generated questions and responses

#### Example using `curl`:

```bash
curl -X POST -F "image=@path/to/your/image.png" http://localhost:5000/analyze
