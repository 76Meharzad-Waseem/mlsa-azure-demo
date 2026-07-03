# MLSA Azure Deployment Demo

This project demonstrates a complete CI/CD pipeline that automatically builds and deploys a web application to **Azure App Service** using **GitHub Actions**, as part of the Microsoft Learn Student Ambassadors (MLSA) program requirements.

## 🚀 Live Site

[msa-demo-77-hqashcbne2embreh.southeastasia-01.azurewebsites.net](https://msa-demo-77-hqashcbne2embreh.southeastasia-01.azurewebsites.net)

## 🛠️ Tech Stack

- **Hosting:** Azure App Service (Linux, F1 Free Tier)
- **CI/CD:** GitHub Actions
- **Frontend:** Static HTML

## 📋 Deployment Workflow

The deployment is fully automated via GitHub Actions. On every push to the `main` branch, the workflow:

1. Checks out the repository
2. Uploads the app as a build artifact
3. Authenticates to Azure using OIDC (`azure/login`)
4. Deploys the app to Azure App Service using `azure/webapps-deploy`

Workflow file: [`.github/workflows/main_msa-demo-77.yml`](.github/workflows/main_msa-demo-77.yml)

## ✅ Deployment Verification

### GitHub Actions — Successful Build & Deploy

The workflow runs successfully on every push, completing both the `build` and `deploy` jobs.

### Azure Deployment Center

The screenshot below confirms the successful deployment as recorded in Azure's Deployment Center, linked directly to this GitHub repository.

![Deployment Center](.github/workflows/Screenshot%202026-07-03%20184221.png)

## 📂 Project Structure
mlsa-azure-demo/
├── .github/
│   └── workflows/
│       └── main_msa-demo-77.yml
├── index.html
├── Screenshot 2026-07-03 184221.png
└── README.md

## 👤 Author

**Meharzad Waseem**
GitHub: [@76Meharzad-Waseem](https://github.com/76Meharzad-Waseem)

---

*This project was created as part of the Microsoft Learn Student Ambassadors (MLSA) program to demonstrate cloud deployment and CI/CD skills using Microsoft Azure.*
