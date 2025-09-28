#  Task 1: Automate Code Deployment Using CI/CD Pipeline (GitHub Actions)

## Objective  
Set up a CI/CD pipeline to **build and deploy a Node.js web application** using **GitHub Actions** and **DockerHub**. This pipeline will automate the process of testing, building, and deploying the application whenever changes are pushed to the **main branch**.

---

## Tools & Technologies  
- **GitHub** → Source code hosting & workflow triggers  
- **GitHub Actions** → CI/CD automation platform  
- **Node.js** → Sample web application  
- **Docker** → Containerization of the app  
- **DockerHub** → Registry to store & deploy container images  

---



## CI/CD Pipeline Workflow  

The pipeline is defined inside   './main.yml'.

### 🔹 Trigger  
- Runs **on every push** to the `main` branch.

### 🔹 Jobs  
1. **Build & Test**  
   - Install dependencies  
   - Run tests (`npm test`)  

2. **Docker Build & Push**  
   - Build Docker image  
   - Login to **DockerHub** using GitHub Secrets  
   - Push image to **DockerHub**  
