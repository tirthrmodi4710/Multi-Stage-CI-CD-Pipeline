# 🚀 Multi-Stage CI/CD Pipeline

---

## 📌 Project Overview

This project demonstrates a Sequential Multi-Environment CI/CD Pipeline using Jenkins and modern DevOps tools.

The pipeline automates the complete software delivery lifecycle from code integration, quality analysis, artifact management, and deployment across multiple environments (DEV → STAGE → PROD).

The workflow follows the **“Build Once, Deploy Many”** approach to ensure reliable, controlled, and production-ready releases.

---

## 🛠️ Technologies Used

- Jenkins  
- GitHub  
- AWS EC2  
- SonarQube  
- Nexus Repository Manager  

---

## 🚀 Sequential Multi-Environment CI/CD Pipeline Workflow

1. Developer pushes latest application code to GitHub repository.  

2. Jenkins pipeline automatically fetches the latest code and starts the CI/CD process.  

3. SonarQube performs code quality and security analysis to validate the application.  

4. Jenkins builds the application artifact and stores the versioned build in Nexus Repository Manager.  

5. The same validated artifact is automatically deployed to the DEV environment for initial testing.  

6. After DEV validation, manual approval is taken to promote the same artifact to the STAGE environment for QA/UAT testing.  

7. Once STAGE testing is completed successfully, another manual approval is taken for PROD deployment.  

8. Jenkins then deploys the exact same tested artifact from Nexus to the PROD environment, ensuring consistency across all environments.  

9. This workflow follows the “Build Once, Deploy Many” approach for controlled, reliable, and production-ready releases.  

---

## 📂 Project Structure

multi-stage-ci-cd-pipeline/
│
├── Jenkinsfile           # CI/CD pipeline configuration  
├── screenshots/          # Jenkins pipeline screenshot    
└── README.md

---

## 📸 Pipeline Screenshot

(Add your Jenkins pipeline screenshot here)

---

## 💡 Key Concepts Implemented

- Sequential multi-environment deployment  
- Build Once, Deploy Many strategy  
- Artifact versioning and promotion  
- Code quality validation using SonarQube  
- Centralized artifact storage using Nexus  
- Controlled production deployment with manual approvals  

---

## 🎯 Outcome

- Improved deployment reliability  
- Reduced manual deployment effort  
- Ensured artifact consistency across environments  
- Implemented controlled release workflow for production deployments  

---

## 👨‍💻 Author

Tirth R. Modi  
