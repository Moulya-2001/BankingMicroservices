# 🏦 Banking Microservice - CI/CD Automation (Midterm Project)

## 📌 Project Overview
This project automates the **build, test, and deployment** process for a Banking Microservice application using **Git, Maven, Jenkins, Docker, and Ansible**.  
The automation ensures that changes to the code are built, tested, containerized, and deployed to a production server with minimal manual intervention.

---

## ⚙ Tech Stack
- **Version Control**: Git & GitHub
- **Build Tool**: Maven
- **CI/CD**: Jenkins
- **Containerization**: Docker
- **Automation**: Ansible
- **Testing**: JUnit
- **Notifications**: Email
- **Web Server**: Apache (installed via Ansible)


## 🚀 Workflow
1. **Code Management**
   - Create GitHub repo: `BankingMicroservice`
   - Create separate branches for each developer[dev1,dev2]
   - Merge reviewed code into `master` branch

2. **Build Automation (Maven)**
   - Jenkins triggers build on master branch update
   - Runs **Maven clean compile test package**
   - Generates JAR file in `target/`

3. **Docker Automation**
   - Builds a Docker image with unique tag
   - Runs container with the latest image

4. **Testing & Notifications**
   - Runs unit tests
   - Sends email notification if tests fail

5. **Production Deployment (Ansible)**
   - **Installs Java and Apache HTTP Server on web servers**
   - Starts Apache service
   - Deploys Docker container

---

## 🖥 Deployment Instructions

### 1️⃣ Prerequisites
- **Production Server**: Ubuntu
- Installed: Git, Docker, Ansible, Jenkins
- GitHub repository with project code

### 2️⃣ Clone Repository
```bash
git clone https://github.com/<your-username>/BankingMicroservice.git
cd BankingMicroservice
