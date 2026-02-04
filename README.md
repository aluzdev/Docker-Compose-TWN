# 🐳 MongoDB + Node.js Profile Manager

This project demonstrates a containerized full-stack environment. It uses **Docker Compose** to orchestrate a MongoDB database and a MongoExpress administration interface, which connects to a Node.js user profile application.

---

## 🚀 Features

- **Containerized Database:** MongoDB runs in an isolated environment.
- **Database GUI:** Includes MongoExpress for easy data visualization.
- **Full-Stack Integration:** A Node.js frontend/backend that persists user profile data.

---

## 🛠 Prerequisites

Before you begin, ensure you have the following installed:

- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [Node.js](https://nodejs.org/) (for running the local server)

---

## 🏃 Getting Started

### 1. Spin up the Database

Run the following command to start the MongoDB and MongoExpress containers:

```bash
docker-compose -f mongo.yaml up -d
```

Note: The `-d` flag runs the containers in "detached" mode so they stay running in the background.

### 2. Start the Application

Ensure your Node.js environment is ready, then launch the server:

```bash
node server.js
```

### 3. Access the Project

Once the services are running, you can access them at:

- **User Interface:** http://localhost:3000
- **MongoExpress (DB Admin):** http://localhost:8081

---

### Pro-Tip for GitHub

If you are using the GitHub web editor, make sure you are in the **"Edit"** tab and not the **"Preview"** tab when pasting. Also, ensure there is a blank line before and after every triple backtick (` ` `) to prevent the code from bleeding into the regular text.

**Would you like me to also provide the `mongo.yaml` code in a copy-paste format to ensure your ports match the ones listed above?**

_You can access the mongo-express under localhost:8080 from your browser_

Step 2: in mongo-express UI - create a new database "user-account"

Step 3: in mongo-express UI - create a new collection "users" in the database "user-account"

Step 4: start node server

    cd app
    npm install
    node server.js

Step 5: access the nodejs application from browser

    http://localhost:3000

#### To build a docker image from the application

    docker build -t my-app:1.0 .

The dot "." at the end of the command denotes location of the Dockerfile.
