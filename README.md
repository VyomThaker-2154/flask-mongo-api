# Task Manager Application

A simple task management application built with Flask, MongoDB, and HTML/JavaScript.

## Features

- Create, read, update, and delete tasks
- Modern and responsive UI
- RESTful API backend
- MongoDB database integration

## Prerequisites

- Python 3.7+
- MongoDB installed and running locally
- pip (Python package manager)

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Make sure MongoDB is running on your local machine
4. Create a `.env` file with your MongoDB connection string (default is already set)

## Running the Application

1. Start the Flask server:
   ```bash
   python app.py
   ```
2. Open your browser and navigate to `http://localhost:5000`

## API Endpoints

- GET `/api/tasks` - Get all tasks
- POST `/api/tasks` - Create a new task
- PUT `/api/tasks/<task_id>` - Update a task
- DELETE `/api/tasks/<task_id>` - Delete a task

## Project Structure

- `app.py` - Flask application and API endpoints
- `templates/index.html` - Frontend interface
- `requirements.txt` - Python dependencies
- `.env` - Environment variables #   f l a s k - m o n g o - a p i  
 