# 🟢 Serverless CRUD API using AWS API Gateway, Lambda & DynamoDB

This project is a fully serverless task management API built using the AWS Console (no frameworks or deployment tools). It supports basic CRUD operations on a DynamoDB table (`sahildemo`) using AWS SDK v3.

---

## ✅ Features

- 🧠 Built with **Node.js** and **AWS SDK v3**
- 🗃️ Stores data in **DynamoDB** table (`sahildemo`)
- ⚙️ Uses **Lambda** for all CRUD logic
- 🌐 Exposed via **API Gateway** (REST)
- 🔐 Secured with **IAM roles**
- 📊 Logs visible via **CloudWatch**

---

## 📂 Project Structure

aws-serverless-crud-api/
├── index.mjs # Lambda handler with CRUD logic
└── README.md # Project description

---

## 📬 Sample API Requests (Postman)

### ➕ Create a Task (POST)
POST /tasks
Content-Type: application/json

{
"name": "Learn AWS",
"completed": false
}

### 📥 Get All Tasks (GET)
GET /tasks

### ✏️ Update a Task (PATCH)
PATCH /tasks
Content-Type: application/json

{
"id": "<your-task-id>",
"name": "Learn AWS Lambda",
"completed": true
}

### ❌ Delete a Task (DELETE)
DELETE /tasks
Content-Type: application/json

{
"id": "<your-task-id>"
}
---

## 🚀 Deployed via AWS Console

- ✅ No CLI, no IaC tools (like CDK/Terraform)
- ✅ All resources created using AWS web console
- ✅ Fully working and tested with Postman

---

## 📌 Author

**Sahil Shakya**

---
