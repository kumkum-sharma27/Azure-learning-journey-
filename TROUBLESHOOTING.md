# 🔧 Azure Troubleshooting Log

Welcome to my Azure Troubleshooting Log.

This document captures the real-world issues I encountered while performing Azure hands-on labs as part of my Azure learning journey. Rather than only documenting successful deployments, I also record the problems I faced, how I investigated them, and the solutions I applied.

**Purpose**
- 📖 Document real Azure troubleshooting scenarios
- 🛠️ Build practical problem-solving skills
- 📚 Create a personal knowledge base
- 💼 Showcase Azure support experience for future interviews

---

# 📋 Troubleshooting Index

| # | Azure Service | Issue | Status |
|---|---------------|--------|--------|
| 1 | Azure App Service | Deployment failed due to regional quota limitation | ✅ Resolved |
| 2 | Azure App Service | Unable to create Basic App Service Plan | ✅ Resolved |
| 3 | Azure Virtual Machine | Unable to access VM through Azure Portal | ✅ Resolved |
| 4 | Azure Virtual Machine | Understanding SSH connectivity | ✅ Resolved |
| 5 | Azure Subscription | Free subscription limitations | ✅ Resolved |

---

# 1️⃣ Azure App Service – Regional Quota Limitation

## 🛑 Issue

Azure App Service deployment failed because the selected Azure region did not have sufficient quota available for my subscription.

---

## 🔍 Root Cause

- Compute quota was unavailable in the selected region.
- A quota increase request had already been submitted but was still pending approval.

---

## ✅ Resolution

- Selected another Azure region with available capacity.
- Switched from the **Basic** pricing tier to the **Free (F1)** App Service Plan.
- Successfully redeployed the web application.

---

## ✔ Verification

- Web App deployed successfully.
- Application was accessible through the Azure-generated URL.

---

## 💡 Key Learning

- Azure resource quotas vary by region.
- Always verify regional availability before deployment.
- Free (F1) App Service Plans can be useful for learning and testing.

---

# 2️⃣ Azure App Service – Basic Plan Limitation

## 🛑 Issue

Unable to create an App Service using the Basic pricing tier.

---

## 🔍 Root Cause

The selected subscription did not have sufficient quota for the Basic App Service Plan.

---

## ✅ Resolution

Used the **Free (F1)** App Service Plan instead.

---

## ✔ Verification

App Service was successfully created.

---

## 💡 Key Learning

Subscription type and pricing tier directly affect available Azure resources.

---

# 3️⃣ Azure Virtual Machine – Portal Access

## 🛑 Issue

Expected to access the Ubuntu Virtual Machine using a graphical interface.

---

## 🔍 Root Cause

Ubuntu Azure Virtual Machines are managed primarily through SSH and do not provide a graphical desktop by default.

---

## ✅ Resolution

Connected to the VM using SSH.

---

## ✔ Verification

Successfully logged into the VM and executed Linux commands.

---

## 💡 Key Learning

Linux Virtual Machines are commonly administered through SSH rather than graphical desktop environments.

---

# 4️⃣ Azure Virtual Machine – SSH Connection

## 🛑 Issue

Initially unfamiliar with how to connect to a Linux VM hosted in Azure.

---

## 🔍 Root Cause

Lack of prior hands-on experience with Linux virtual machines.

---

## ✅ Resolution

Used Azure's SSH connection method to securely connect to the Ubuntu Virtual Machine.

Executed basic Linux commands to verify connectivity.

---

## ✔ Verification

Successfully connected to the VM using SSH.

---

## 💡 Key Learning

SSH is the standard method for securely managing Linux virtual machines hosted in Azure.

---

# 5️⃣ Azure Subscription – Free Tier Limitations

## 🛑 Issue

Certain Azure resources could not be deployed using the preferred configuration.

---

## 🔍 Root Cause

Azure Free subscriptions include quota limits and service restrictions.

---

## ✅ Resolution

- Used supported Azure regions.
- Selected the Free (F1) pricing tier when appropriate.
- Submitted quota increase requests where required.

---

## ✔ Verification

Successfully completed the hands-on lab using supported configurations.

---

## 💡 Key Learning

Understanding subscription limits is an important part of Azure administration and troubleshooting.

---

# 📚 Overall Learnings

Throughout these hands-on labs, I gained practical experience in:

- ☁️ Azure Resource Deployment
- 🔧 Troubleshooting Azure Services
- 🌍 Regional Availability
- 📊 Subscription Quotas
- 🖥️ Azure Virtual Machines
- 🔐 SSH Connectivity
- 🌐 Azure App Service
- 📝 Azure Documentation

---

# 🚀 Future Troubleshooting Scenarios

As I continue my Azure learning journey, this document will be updated with additional troubleshooting scenarios, including:

- ⏳ Azure Storage
- ⏳ Azure Virtual Network (VNet)
- ⏳ Network Security Groups (NSG)
- ⏳ Azure Monitor
- ⏳ Azure RBAC
- ⏳ Azure Backup
- ⏳ Azure Functions
- ⏳ Azure Container Apps

---

> **Note:** All issues documented here were encountered and resolved during my own Azure hands-on practice while preparing for Azure Administration and Application Support roles.
