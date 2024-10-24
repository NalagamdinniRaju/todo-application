# To-Do List Application

## Overview
This project is a simple **To-Do List Application** built using the **MERN stack** (MongoDB, Express, React, Node.js). It allows users to create, update, and delete tasks while tracking the completion status of each task. The project also integrates real-time notifications using `react-toastify` for task-related updates such as task creation, deletion, and modification.

## Features
- **Add Tasks**: Users can add new tasks to the list.
- **Update Tasks**: Users can edit the title of tasks and mark tasks as completed or not completed.
- **Delete Tasks**: Users can remove tasks from the list.
- **Real-time Feedback**: Notifications are shown for success or error operations.
- **CRUD Operations**: The application supports Create, Read, Update, and Delete (CRUD) functionalities with the backend connected to MongoDB.

## Tech Stack
- **Frontend**: React.js with `react-toastify` for notifications, `react-icons` for icons.
- **Backend**: Node.js, Express.js.
- **Database**: MongoDB.
- **API**: Axios is used for making API calls between the frontend and backend.
- **Additional Libraries**: 
  - `mongoose`: For MongoDB object modeling.
  - `dotenv`: To handle environment variables.
  - `cors`: Middleware to allow cross-origin resource sharing.



## Installation

### Prerequisites
- **Node.js** (v14+)
- **MongoDB** (running locally or via a service like MongoDB Atlas)

### Clone the Repository
```bash
git clone https://github.com/yourusername/todo-app.git
cd todo-app
```

### Backend Setup
1. **Install dependencies** for the backend:
   ```bash
   cd server
   npm install
   ```

2. **Create a `.env` file** in the `server` directory and add the following:
   ```bash
   MONGO_URI=mongodb://localhost:27017/todolist
   ```

3. **Run the backend server**:
   ```bash
   npm start
   ```
   The backend will be running on `http://localhost:5000`.

### Frontend Setup
1. **Install dependencies** for the frontend:
   ```bash
   cd client
   npm install
   ```

2. **Run the frontend**:
   ```bash
   npm start
   ```
   The frontend will be running on `http://localhost:3000`.

## Usage
1. After setting up both the frontend and backend, navigate to `http://localhost:3000` to view the application.
2. You can add a new task using the input form.
3. Each task in the list can be marked as completed, edited, or deleted.
4. Toast notifications will appear to provide feedback for operations (task added, updated, or deleted).

## API Endpoints

- `GET /api/tasks`: Fetch all tasks.
- `POST /api/tasks`: Create a new task.
- `PUT /api/tasks/:id`: Update an existing task.
- `DELETE /api/tasks/:id`: Delete a task.

## Additional Notes
- **React Icons** are used for edit, save, and delete task buttons.
- **MongoDB** is used to persist tasks, and the **Mongoose** library is used to define the schema for tasks.
- **React Toastify** is integrated for success/error messages when interacting with tasks.


## License
This project is licensed under the MIT License.

---
