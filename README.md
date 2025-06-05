Task Manager App
A simple task manager built with React, Vite, and Tailwind CSS. Users can view, add, mark as completed, and delete tasks, with filtering for all, pending, or completed tasks.
Features

View a list of tasks
Add new tasks (with validation to prevent empty titles)
Mark tasks as completed (toggles completion status)
Delete tasks
Filter tasks by All, Pending, or Completed
Responsive design with Tailwind CSS
Completed tasks are styled with a green background and strikethrough

Setup Instructions

Initialize a Vite project:npm create vite@latest task-manager -- --template react
cd task-manager
npm install


Install Tailwind CSS:npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p


Configure tailwind.config.js:/** @type {import('tailwindcss').Config} */
export default {
  content: ['./index.html', './src/**/*.{js,jsx}'],
  theme: { extend: {} },
  plugins: [],
}


Add Tailwind directives to src/index.css:@tailwind base;
@tailwind components;
@tailwind utilities;


Replace the contents of src with the provided files (App.jsx, TaskForm.jsx, TaskList.jsx, TaskFilter.jsx).
Update index.html with the provided HTML.
Run the app:npm run dev


Open the app in your browser at http://localhost:5173.

Usage

Enter a task title in the input field and click "Add" to create a new task.
Click a task title to toggle its completion status.
Click "Delete" to remove a task.
Use the filter buttons to view All, Pending, or Completed tasks.
Empty task titles are prevented with an alert.

Notes

Tasks are stored in a hardcoded array in App.jsx.
No backend is required; state is managed with React's useState.
The app is styled with Tailwind CSS for a clean, responsive UI.

