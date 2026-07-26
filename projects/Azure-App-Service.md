# Azure App Service Deployment

## 📌 Project Overview
This project demonstrates deploying a web application using **Azure App Service**.  
It covers subscription setup, quota management, provider registration, and verifying successful deployment.

---

## 🎯 Objective
- Create an Azure App Service  
- Deploy a sample web application  
- Verify successful deployment  
- Understand Platform as a Service (PaaS)  

---

## ☁️ Azure Services Used
- Azure App Service  
- Resource Group  
- Subscription Quota Management  

---

## 🚀 Deployment Steps
1. Signed in to Azure Portal  
2. Created a Resource Group  
3. Selected Azure App Service  
4. Configured the Web App (runtime stack, OS, region)  
5. Registered the **Microsoft.Web** provider  
6. Requested quota increase for **Compute-VM (cores-vCPUs)**  
7. Created the App Service Plan  
8. Successfully deployed the web application  
9. Verified the application using the provided URL  

---

## 📷 Screenshot Gallery

### Azure App Service Overview
![Azure App Service Overview](../images/app-service-overview.png)

### Running Web Application
![Running Web Application](../images/web-app-running.png)

---

## 🛠 Skills Demonstrated
- Azure App Service setup  
- Subscription quota management  
- Resource provider registration  
- Web Application Deployment  
- Azure Portal navigation  
- PaaS concepts  

---

## ✅ Outcome
Successfully deployed and verified a web application using Azure App Service.  
The app is live at the generated Azure URL, confirming the deployment process was completed end-to-end, including resolving quota and provider registration challenges.

---

## ⚠️ Challenge Faced

While deploying the Azure App Service, the deployment initially failed because the selected Azure region did not have sufficient available quota for my subscription. Although I had already requested a quota increase, the request was still pending approval, preventing the deployment from completing in that region.

### Resolution

To continue the hands-on exercise without waiting for the quota approval:

- Selected another Azure region with available capacity.
- Changed the App Service Plan pricing tier from **Basic** to the **Free (F1)** tier, which was supported by my subscription.
- Redeployed the application successfully.

### Key Learning

- Azure resource availability can vary by region and subscription quotas.
- If deployment fails due to quota limitations, selecting another supported region can resolve the issue.
- Choosing an appropriate pricing tier based on subscription limits is important during deployment.
- Understanding Azure quotas and regional availability is an essential part of troubleshooting Azure deployments.
