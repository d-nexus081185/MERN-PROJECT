Employee Record Web App

This project is a simple Employee Record Management web application built using the MERN stack (MongoDB, Express, React, Node.js). It allows users to manage employee records by adding, viewing, editing, and deleting records.

Features

Frontend: Built with React and Vite for a fast and responsive user interface.

Backend: Powered by Express.js, providing RESTful API endpoints for CRUD operations.

Database: MongoDB to store and retrieve employee data efficiently.

Styling: Flexible and modern design for a seamless user experience.

Prerequisites

Before you begin, ensure you have the following installed on your system:

Node.js (v14 or later)

npm or yarn

MongoDB (local or cloud instance, e.g., MongoDB Atlas)

How To Run

1. Clone the Repository

git clone https://github.com/d-nexus081185/MERN-PROJECT.git
cd MERN-PROJECT

2. Backend Setup

Navigate to the backend directory:

cd MERN-PROJECT/backend

Create a file named config.env in the server folder with the following content:

MONGO_URI=mongodb+srv://<username>:<password>@cluster0.wyi99.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
PORT=5000

Replace <username> and <password> with your MongoDB Atlas credentials.

Install the backend dependencies:

npm install

Start the backend server:

npm start

The server will run on http://localhost:5000.

3. Frontend Setup

Navigate to the client directory:

cd MERN-PROJECT/client

Install the frontend dependencies:

npm install

Start the development server:

npm run dev

The web server will run on http://localhost:3000.

Cloud Deployment and DevOps Practices

This project is part of learning how to deploy a 3-tier MERN stack application to the cloud using AWS as the cloud platform. The deployment process will include the following steps:

Cloud Deployment: The application will be deployed to AWS services such as EC2, Elastic Beanstalk, or AWS Lambda.

CI/CD Pipeline: DevOps best practices will be applied by creating a Continuous Integration and Continuous Deployment (CI/CD) pipeline using GitHub Actions or GitLab CI/CD. This will ensure automated testing, building, and deployment.

Containerization: The application will be dockerized by adding a Dockerfile. A Docker image will be created and run as a container, enabling portability and scalability.

Project Structure

MERN-PROJECT/
├── backend/
│   ├── models/       # Database models
│   ├── routes/       # API routes
│   ├── server.js     # Main server file
│   └── config.env    # Environment configuration
├── client/
│   ├── src/          # React source files
│   ├── public/       # Static assets
│   └── vite.config.js # Vite configuration
└── README.md         # Project documentation

API Endpoints

GET /api/employees: Fetch all employees.

POST /api/employees: Add a new employee.

PUT /api/employees/:id: Update an existing employee.

DELETE /api/employees/:id: Delete an employee.