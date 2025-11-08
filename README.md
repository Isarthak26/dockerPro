This project is a complete walkthrough of building, containerizing, and deploying a full-stack application from scratch. The steps follow the flow of the video “0 to Production (VPS)” and include backend setup, frontend setup, Dockerization, Docker Compose, and final deployment on a VPS.

✅ What You Will Build

A minimal Node.js + Express backend

A React (Vite) frontend

Full communication between backend ↔ frontend

Backend and frontend Docker containers

A Docker Compose setup to run everything with one command

Deployment on a VPS (Hostinger used in the demo)

Domain mapping + DNS configuration

Debugging real bugs introduced intentionally in the project

✅ Tech Stack

Node.js + Express

React + Vite

Docker & Docker Compose

VPS (Ubuntu 24.04 LTS)

Basic Networking + DNS

✅ Project Structure
project/
 ├── server/      # Node.js backend
 └── client/      # React frontend

✅ Backend Summary

Initialize project using npm init -y

Add dependencies:

npm install express cors


Setup:

Use "type": "module" for ES modules

Create index.js with:

Express server

CORS middleware

JSON middleware

Basic API route: /api/message

Start script added:

npm run start


Verified using Postman (GET /api/message)

✅ Frontend Summary

Create React project using Vite

npm create vite@latest


Clean default template

Add simple UI:

Title

Display fetched backend message

Fetch data using:

useEffect

fetch("http://localhost:4000/api/message")

State management using useState

✅ CORS & Proxy

Explanation of why CORS is necessary

When to use proxy

Common mistakes during frontend ↔ backend communication

✅ Dockerization

Both backend and frontend are containerized separately.

Backend Docker:

Create Dockerfile

Copy project files

Install dependencies

Expose port

Run server

Frontend Docker:

Build React app

Serve with a lightweight server (like nginx)

Expose frontend port

✅ Docker Compose

Combine both containers in one docker-compose.yml

Enable:

Shared network

Container-to-container communication

Single command startup:

docker compose up

✅ Deployment on VPS

Purchase VPS (Hostinger used in demo)

Choose raw Ubuntu machine

Access via browser-based SSH terminal

Steps include:

Install Docker & Docker Compose

Pull code from GitHub

Run stack using docker compose

Configure domain + DNS

Verify app is publicly live

✅ Key Learning Highlights

Full-stack workflow from scratch

Real debugging as bugs are intentionally introduced

Clean deployment without CI/CD pipelines

Understanding environment variables

Container networking fundamentals
