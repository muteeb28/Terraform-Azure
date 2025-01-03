## Infrastructure as Code (IaC)

### What is Infrastructure as Code (IaC)?
- Provisioning your infrastructure through code.
- Instead of manually creating resources via a cloud console (e.g., Azure Portal), you automate the process using code.

---
### Why Use Infrastructure as Code?
- **Manual Provisioning (Azure Console):**
  - Simple drag-and-drop for infrastructure.
  - Good for personal projects or learning.
  
- **Challenges in Scaling:**
  - Provisioning for multiple environments (e.g., Dev, QA, Prod) can take hours.
  - Managing hundreds of servers manually is time-consuming and error-prone.
  
- **Cost Efficiency:**
  - Decommissioning resources daily reduces costs but is impractical without automation.
  - IaC automates infrastructure lifecycle (create, manage, destroy).

- **Common Problems IaC Solves:**
  - Identical environments (avoid "works on my machine" issues).
  - Automate provisioning for reliability, efficiency, and security.

---
### Benefits of IaC:
- **Consistency:** Identical environments reduce drift.
- **Cost Tracking:** Easier to monitor and control cloud spending.
- **Reusable Code:** Write once, deploy many times.
- **Time Saving:** Automates infrastructure deployment.
- **Error Reduction:** Minimizes human error.
- **Version Control:** Infrastructure changes are tracked in Git.
- **Automated Cleanup:** Schedule resource destruction.
- **Developer Productivity:** Focus on app development.
- **Troubleshooting:** Easily replicate production environments.

---
### What is Terraform?
- **Definition:** Terraform is an IaC tool that automates infrastructure provisioning and management.
- **Workflow:**
  1. **Write:** Define infrastructure using Terraform configuration files.
  2. **Run:** Execute Terraform commands.
  3. **Provision:** Terraform calls cloud provider APIs to create infrastructure using its provider plugins.

---
### Terraform Workflow Phases:
1. **Init:** Initialize Terraform.
2. **Validate:** Check for syntax errors.
3. **Plan:** Preview infrastructure changes.
4. **Apply:** Provision infrastructure.
5. **Destroy:** Remove infrastructure.

---
### Day 2 Task: Install Terraform
- **Install Instructions:** [Terraform Installation Guide](https://developer.hashicorp.com/terraform/install)
- **Common Installation Error (macOS):**
  ```bash
  brew install hashicorp/tap/terraform
  # Error: No developer tools installed.
  # Fix:
  xcode-select --install  
  ```
  - A pop-up will appear. Install command line tools.

- **Post-Install Commands:**
  ```bash
  terraform -install-autocomplete
  alias tf=terraform
  terraform -version
  ```

