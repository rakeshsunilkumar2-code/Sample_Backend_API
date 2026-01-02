***Simple Backend API***
**Overview**

A minimal backend API built with Node.js & Express.
It exposes a single endpoint /sayHello and is automatically deployed to a VM using GitHub Actions.

Runs on Port 80
Automated CI/CD
No secrets in repo or VM
No manual deployment

***API Endpoint***
**GET /sayHello**

*Response*

{
  "message": "Hello User."
}

*Run Locally*

npm install
sudo node index.js


*Test:*

curl http://localhost/sayHello

**Deployment**

Triggered on push to main
Uses GitHub Actions
Secure SSH via GitHub Secrets
Fresh clone on VM (no git pull)

**Screenshot**


<img width="325" height="94" alt="screenshot" src="https://github.com/user-attachments/assets/9b6685df-7e20-46e1-bbd2-18023f39172c" />


curl http://20.102.98.247/sayHello

**Response**

{ "message": "Hello User." }

**Author**
Rakesh Sunilkumar
