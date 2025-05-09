# Task Manager Application 🚀

A modern task management application built with Flask, MongoDB, and HTML/JavaScript. This application demonstrates a full-stack implementation of a RESTful API with a responsive frontend interface.

## ✨ Features

- **CRUD Operations**: Create, Read, Update, and Delete tasks
- **Modern UI**: Clean and responsive interface built with Bootstrap
- **RESTful API**: Well-structured backend API endpoints
- **Real-time Updates**: Instant UI updates when tasks are modified
- **Data Persistence**: MongoDB integration for reliable data storage

## 🛠️ Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.7 or higher
- MongoDB Community Server
- pip (Python package manager)

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/task-manager.git
   cd task-manager
   ```

2. Install required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure MongoDB:
   - Make sure MongoDB service is running on your machine
   - Create a `.env` file in the project root:
     ```
     MONGODB_URI=mongodb://localhost:27017/taskdb
     ```

## 🚀 Running the Application

1. Start the Flask server:
   ```bash
   python app.py
   ```

2. Access the application:
   - Open your web browser
   - Navigate to `http://localhost:5000`
   - The task manager interface should now be visible

## 🔌 API Documentation

### Endpoints

| Method | Endpoint | Description | Request Body |
|--------|----------|-------------|--------------|
| GET | `/api/tasks` | Retrieve all tasks | - |
| POST | `/api/tasks` | Create a new task | `{"title": "string", "description": "string"}` |
| PUT | `/api/tasks/<task_id>` | Update a task | `{"title": "string", "description": "string"}` |
| DELETE | `/api/tasks/<task_id>` | Delete a task | - |

### Example API Usage

```bash
# Get all tasks
curl http://localhost:5000/api/tasks

# Create a new task
curl -X POST http://localhost:5000/api/tasks \
  -H "Content-Type: application/json" \
  -d '{"title": "New Task", "description": "Task description"}'

# Update a task
curl -X PUT http://localhost:5000/api/tasks/task_id \
  -H "Content-Type: application/json" \
  -d '{"title": "Updated Task"}'

# Delete a task
curl -X DELETE http://localhost:5000/api/tasks/task_id
```

## 📁 Project Structure

```
task-manager/
├── app.py              # Flask application and API endpoints
├── templates/
│   └── index.html      # Frontend interface
├── requirements.txt    # Python dependencies
├── .env               # Environment variables
└── README.md          # Project documentation
```

## 🔧 Technology Stack

- **Backend**: Flask (Python)
- **Database**: MongoDB
- **Frontend**: HTML, JavaScript, Bootstrap
- **API**: RESTful architecture
- **Environment**: python-dotenv
- **CORS**: flask-cors

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🐛 Troubleshooting

If you encounter any issues:

1. Ensure MongoDB is running:
   ```bash
   mongod --version
   ```

2. Check if Flask server is running without errors
3. Verify your `.env` file configuration
4. Check browser console for frontend errors

For more help, please open an issue in the repository.

 