# 🤖 AI SQL Agent — Natural Language Database Assistant








## An AI-powered database assistant that allows users to interact with a MySQL database using natural language instead of writing SQL queries.

  The system uses an LLM-based AI Agent connected with n8n automation workflows to perform database operations like:

  ✔ Select data
  ✔ Insert records
  ✔ Update records
  ✔Delete records

All operations are executed automatically by the AI agent based on user instructions.

# 🚀 Project Overview

This project demonstrates how Large Language Models (LLMs) can be integrated with automation tools and databases to build intelligent systems.

Instead of writing SQL queries manually, users can simply ask:

Show all customers from France
Add a new employee
Update employee email
Delete employee record

The AI agent understands the request and executes the correct database operation.

# 🧠 System Architecture
User Query
   │
   ▼
n8n Chat Trigger
   │
   ▼
AI Agent (LLM)
   │
   ├── Memory (Conversation Context)
   │
   ├── MySQL Tools
   │     ├─ Select rows
   │     ├─ Insert rows
   │     ├─ Update rows
   │     └─ Delete rows
   │
   ▼
MySQL Database
<img width="1920" height="1080" alt="workflow" src="https://github.com/user-attachments/assets/b79af020-3c9b-4170-b2ed-f9045f4e4966" />


The AI agent acts as a controller that interprets user queries and decides which tool to use.

# ✨ Features

🧠 Natural language database interaction
⚡ AI-powered query interpretation
📊 MySQL CRUD operations
🔄 Automated workflow using n8n
💬 Conversational AI interface
🗂 Real database operations executed via tools

# 🛠 Technologies Used
Technology	Purpose
n8n	Workflow automation
Google Gemini / LLM	AI reasoning
MySQL	Database
AI Agent Tools	Database interaction
JSON Workflow	Automation pipeline
💬 Example AI Commands

The AI agent understands natural language instructions.

🔎 Retrieve Data
Show all customers from the customers table who are located in France.
➕ Insert Record
Add a new employee Rahul Sharma with employeeNumber 1113.
✏ Update Record
Update the email of employee 1113 to rahul.ai.engineer@classicmodelcars.com.
❌ Delete Record
Delete the employee with employeeNumber 1113 from the employees table.
⚙ Setup Instructions
1️⃣ Install n8n
npm install -g n8n

Run:

n8n start
2️⃣ Import Workflow

Import the workflow file into n8n.

workflow/n8n_workflow.json
3️⃣ Setup MySQL Database

Import the database schema.

database/mysql_database.sql
4️⃣ Configure Credentials

Add credentials for:

MySQL Database

LLM API (Gemini / other supported model)

# 📂 Project Structure
AI-SQL-Agent
│
├── workflow
│   └── n8n_workflow.json
│
├── database
│   └── mysql_database.sql
│
├── examples
│   └── example_agent_chat.txt
│
└── README.md
# 🎯 Use Cases

AI Database Assistants

Internal company automation tools

Natural language data access

AI backend assistants

AI-driven database management

# 👨‍💻 Author

Omkar Chougule

AI Engineer | Data Analyst | Machine Learning Enthusiast
