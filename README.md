# Azure DevOps Pipelines Studio

This repository contains the target configuration and SRE runtime files compiled by the **Azure DevOps Pipelines Studio** dashboard module.

## 🚀 Description
Author robust pipeline tasks for Azure DevOps. Generate multi-stage YAML pipelines, agent pool targets, secret library links, and sonarqube scans gates.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `//azure-pipelines.yml`
- **Execution Command**: `az pipelines run --name pipeline`
- **Validation Command**: `az pipelines build list`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-devops-pipelines.git
   cd tp-azure-devops-pipelines
   ```

2. **Run Execution Target:**
   ```bash
   az pipelines run --name pipeline
   ```

3. **Verify Runtime Stability:**
   ```bash
   az pipelines build list
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
