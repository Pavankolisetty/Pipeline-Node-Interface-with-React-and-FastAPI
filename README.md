# Pipeline Node Interface with React and FastAPI

This project is a full-stack application to manage pipeline nodes and edges. The system allows users to create and manipulate pipeline graphs, calculate graph metrics (number of nodes, edges), and validate Directed Acyclic Graphs (DAG). The frontend is built using React, and the backend uses Python's FastAPI framework.

## Features

- **Dynamic Node Creation**: Abstracted nodes (Input, Output, Text, LLM) for scalability.
- **Interactive UI**: React-based drag-and-drop interface with dynamic text resizing and variable-based handle generation.
- **Graph Analysis**: FastAPI backend to calculate metrics (number of nodes, edges) and validate DAG structures.
- **Seamless Integration**: Frontend and backend communicate through RESTful APIs with user-friendly alerts.

---

## Project Structure

### **Frontend**
- Built with React and Zustand for state management.
- Provides an interactive drag-and-drop interface for node management.

### **Backend**
- Developed with FastAPI to process graph data.
- Calculates graph metrics and validates DAG structures.

---

## Prerequisites

Make sure you have the following installed:
- **Node.js** (>=16.x)
- **Python** (>=3.9)
- **npm** (Node Package Manager)

---

## Installation

### **1. Clone the Repository**
```bash
git clone https://github.com/<your-username>/pipeline-node-management.git
cd pipeline-node-management


##Setting up Frontend 
cd frontend
npm install
npm start

## Setting backend 
cd ../backend
pip install -r requirements.txt
uvicorn main:app --reload


##Usage
Start the Frontend:

Open your browser and navigate to http://localhost:3000.
Start the Backend:

The API server will run on http://localhost:8000.
Interact with the Application:

Use the drag-and-drop UI to add nodes and edges.
Click "Submit" to send the pipeline data to the backend.
View the graph metrics (number of nodes, edges, DAG status) in an alert.
