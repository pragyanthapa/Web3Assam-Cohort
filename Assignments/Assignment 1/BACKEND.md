# Task 2: Backend Assignment – Store & Manage User Data in JSON File

## 📌 Overview

This assignment evaluates your ability to build a backend service using **Node.js + Express** (or any equivalent backend framework). You will create APIs that read and write data to a local JSON file, simulating database operations.

---

## 📁 Folder Structure (Submission)

Your submission must follow this structure:

```
/mentee/
   /your-name/
       /Assignment 1/
               (your backend project files)
               README.md
```

All code must remain inside your personal folder.

---

## 🎯 Objective

Create a backend service with APIs that:

* Read user data from a local `users.json` file
* Insert new users into the same JSON file
* Serve the data over HTTP endpoints

---

## 📂 Required Files

Inside your backend project:

```
users.json
server.js (or index.js)
```

Initial `users.json` content (empty array):

```json
[]
```

---

## 🔗 API Requirements

### ✔ **GET /users**

* Returns all users stored in `users.json`
* Response example:

```json
[
  {
    "id": 1,
    "name": "Alice",
    "email": "alice@mail.com"
  }
]
```

### ✔ **POST /users**

* Accepts JSON body:

```json
{
  "name": "Bob",
  "email": "bob@mail.com"
}
```

* Adds the entry to `users.json`
* Auto‑generates `id` (incremental)
* Returns success response

---

## 🛠️ Running Commands (Add these in your README)

Example:

```
npm install
node server.js
```

Using nodemon:

```
npm install
yarn dev
```

(Your commands may vary depending on your setup.)

---

## 📤 Submission Guidelines

1. Fork the repo:

   * **[https://github.com/jishantukripal/Web3Assam-Cohort/](https://github.com/jishantukripal/Web3Assam-Cohort/)**
2. Navigate to:

   ```
   /mentee/your-name/
   ```
3. Create the folder structure:

   ```
   Assignment 1/
   ```
4. Place your backend project inside **Assignment 1**.
5. Include a **README.md** in task2 explaining:

   * How to run your server
   * API endpoints
   * Any optional enhancements you implemented
6. Commit and push changes to your fork.
7. Create a **Pull Request** to the main repository.
8. PR must contain **only your mentee folder changes**.

---

## 🤖 AI Usage Policy

You may use AI assistance **only if you know how to debug issues yourself**.
Your backend **must run without errors**.

---

## 🧪 Evaluation Criteria

| Area              | Details                                  |
| ----------------- | ---------------------------------------- |
| API Functionality | GET & POST endpoints must work correctly |
| File Handling     | JSON reading/writing error-free          |
| Validation        | User input must be validated             |
| Code Quality      | Clean structure, modular, readable       |
| Error Handling    | Proper HTTP status codes + safe fails    |

---

