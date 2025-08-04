🚀 Node.js DevOps Task – Hello Jarvis Server
This project is a simple Node.js HTTP server designed to demonstrate basic DevOps skills, including:

Writing and serving a Node.js app

Containerizing it using Docker

Running basic tests to verify its functionality


📁 Project Structure

📦 DevOps--Task1/

 ┣ 📂 .github/
 
 ┃  ┗ 📂 workflows/
 
 ┃     ┗ 📄 main.yml
 
 ┗ 📂 nodejs-demo-app/
 
    ┣ 📂 tests/
    
    ┃  ┗ 📄 app.test.js 
    
    ┣ 📄 Dockerfile 
    
    ┣ 📄 index.js
    
    ┗ 📄 package.json
    
🧾 Features

Responds with a greeting message on root URL (/)

Returns 404 for other paths

Containerized using Docker

Includes a basic test using built-in http module (no external frameworks)


▶️ How It Works
index.js
Creates a basic HTTP server.

Responds with: 
t
Hello Jarvis This is My DevOps Task
when accessed at /.

🐳 Docker Instructions
1. Build the Docker Image
t
docker build -t nodejs-demo-app .
2. Run the Docker Container

docker run -p 3000:3000 nodejs-demo-app
This maps port 3000 from container to host so you can visit:



http://localhost:3000

✅ Test the Application
Run the Test Script

node tests/app.test.js
Expected Output


Status Code: 200
Body: Hello Jarvis This is My DevOps Task
✅ Test Passed
If the server is not responding or the message doesn't match, you’ll see:


❌ Test Failed
📦 Package Requirements
Install dependencies using:



npm install
Make sure your package.json includes a start script like:

json

"scripts": {
  "start": "node index.js"
}
📤 Submission

Repo Link:
🔗 
