# StudyBuddy - Learning Management Portal

> Welcome to the Learning Management Portal! This application is designed to enhance the learning experience through Artificial Intelligence. Users can engage with course materials, submit various types of assignments, and receive AI-powered assistance. 

## Features

- **Course Content Access**: Interact with diverse educational materials.
- **Assignment Submissions**: Submit multiple types of assignments (MCQs, MSQs, numeric problems, and coding tasks).
- **AI Assistance**: Get AI-powered material summaries, contextual hints, and an interactive document chat feature.
- **Coding Support**: Access hints and assistance for coding assignments.

## Technologies Used

- **Python 3**: Main programming language.
- **FastAPI**: Backend framework for fast and efficient API creation, with built-in validation and documentation.
- **React**: JavaScript library for building user interfaces (frontend).
- **MongoDB**: NoSQL database for data storage.
- **LangChain**: A framework used for building applications powered by Large Language Models (LLMs).

## Prerequisites

To run the app locally, ensure that the following software is installed:

- **Python 3**
- **Pip** (Python package manager)
- **Node.js**
- **Npm** (Node package manager)
- **Java**
- **MongoDB** (Ensure MongoDB server is running)

## Installation Guide

Follow the steps below to set up the development environment:

### 1. Clone the Repository

```bash
git clone https://github.com/De-Sagnik/soft-engg-project-may-2024-se-may-22.git
```
### 2. Install Required Packages
Set up a virtual environment and install the necessary dependencies
```ssh
python -m venv venv

# Activate the virtual environment (on Windows use `venv\Scripts\activate`)
source venv/bin/activate

# Install the dependencies
pip install -r requirements.txt

```
### 3. Set up Environment Variables
Create a .env file in the project's root directory and define the following environment variables:
```
DATABASE = "se_project"
DATABASE_USERNAME = "user"
DATABASE_PASSWORD = "password"
SECRET_KEY = secret_key
ALGORITHM = "HS256"
ACCESS_TOKEN_EXPIRE_MINUTES = 60
GOOGLE_CLIENT_ID = google_client_id
GOOGLE_CLIENT_SECRET = google_client_secret
GOOGLE_REDIRECT_URI = "http://localhost:8000/oauth/callback"
GOOGLE_AI_KEY = "google_ai_key" # Gemini-model API key
```
> **Note**: If you want to use a local database, replace the URI with mongodb://localhost:27017 in the db.py file located in the database folder.

## Running the App
### 1. Starting the Application
Backend
```
python3 main.py
```
Frontend
```
npm install
npm start
```
### 2. Access the App
Open your browser and navigate to: http://localhost:3000

## Project Structure
```
.
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── db.py
│   │   └── ...
├── frontend/
│   ├── src/
│   └── public/
├── requirements.txt
├── package.json
└── .env
```

## License
This project is licensed under the MIT License. See the LICENSE file for more details.


