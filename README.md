# 🔩 Personal Task Manager API

This is a lightweight mock API for a personal task manager. It uses [json-server](https://github.com/typicode/json-server) to simulate a real REST API and serves as the backend for your UI task.

---

## 🚀 Getting Started

### 0. Use the Correct Node Version

This project uses **Node.js v22+**. We recommend using [nvm (Node Version Manager)](https://github.com/nvm-sh/nvm) to manage your Node versions.

#### Install nvm (if not already installed)
Follow the setup instructions here: https://github.com/nvm-sh/nvm#installing-and-updating

#### Switch to correct Node version:
```bash
nvm install 22
nvm use 22
```

If you're using a shell like zsh or bash, the `.nvmrc` file in this repo will automatically set the correct version:
```bash
nvm use
```

---

### 1. Install Dependencies

You’ll need Node.js (v22+) installed.

Or use `npx` without installing globally:

```bash
yarn install
```

### 2. Start the API Server

```bash
yarn start
```

The server will be available at:  
📱 `http://localhost:3001/tasks`

---

## 📦 API Overview

### Get all tasks
```
GET /tasks
```

### Add a new task
```
POST /tasks
```
```json
{
  "title": "My New Task",
  "description": "Task details here",
  "dueDate": "2025-04-20",
  "priority": "medium",
  "status": "todo"
}
```

### Delete a task
```
DELETE /tasks/:id
```

### Get tasks sorted by due date
```
GET /tasks?_sort=dueDate&_order=asc
```

---

## 🥪 Tips

- You can edit `db.json` directly to seed new tasks.
- Use `GET /tasks` with filters or sorts to help implement UI features easily.

---

Happy building! 💻✨
