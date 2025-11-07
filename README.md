# 🎮 Super Mario on Kubernetes using Terraform

## 🧩 Overview

This project demonstrates how to **deploy a containerized version of the Super Mario game** on a **Kubernetes cluster** — with the entire infrastructure provisioned using **Terraform**.  
It showcases the seamless integration of **Infrastructure as Code (IaC)** and **container orchestration** tools to create a modern, automated, and scalable deployment pipeline.

---

## 🚀 Scenario

Imagine a gaming company deploying its **Super Mario** game on Kubernetes using Terraform.  
Terraform sets up the underlying infrastructure, while Kubernetes manages the game’s **deployment, scaling, and reliability**.  
As player demand grows, the company can easily **scale their infrastructure** with Terraform and Kubernetes, ensuring a smooth gaming experience for users worldwide.

---

## 🏗️ Project Description

This project involves:
- Using **Terraform** to provision cloud infrastructure components — including Kubernetes clusters, networking, and storage.
- Deploying the **Super Mario game container** on Kubernetes for scalable and reliable management.
- Demonstrating modern DevOps practices such as **automation**, **IaC**, and **cloud-native application deployment**.

By combining Terraform and Kubernetes, this project ensures:
- ⚙️ **Scalability** – Easily scale deployments based on demand.  
- 🔒 **Reliability** – Managed containerized workloads with high availability.  
- 📦 **Efficiency** – Automated infrastructure provisioning and orchestration.  

---

## 🧠 Key Tools & Technologies

| Tool / Technology | Purpose |
|--------------------|----------|
| **Terraform** | Infrastructure as Code (IaC) for provisioning the Kubernetes cluster |
| **AWS EC2** | Host environment for running Terraform and other dependencies |
| **AWS CLI** | Command-line tool for managing AWS resources |
| **Docker** | Containerization of the Super Mario application |
| **Kubernetes (EKS)** | Orchestration and management of containerized applications |
| **kubectl** | CLI for managing Kubernetes clusters and deployments |
| **S3 Bucket** | Storage backend for Terraform state management |

---

## ⚙️ Infrastructure Workflow

1. **Launch & Configure an EC2 Instance**  
   Provision an AWS EC2 instance to serve as the control node for deploying the setup.

2. **Install and Configure Required Tools**
   - 🐳 **Docker** – For containerization  
   - 🌍 **Terraform** – For infrastructure provisioning  
   - ☁️ **AWS CLI** – For cloud interaction  
   - ⚡ **kubectl** – For Kubernetes management  

3. **Create and Attach IAM Role**  
   Define IAM roles with the required permissions and attach them to the EC2 instance.

4. **Setup an S3 Bucket**  
   Store the Terraform state file to enable collaborative IaC workflows.

5. **Clone Terraform Repository and Initialize Workspace**
   ```
   git clone <terraform-repo-url>
   cd <project-folder>
   terraform init
   ```
6. **Validate & Execute Terraform Plan**
```
terraform plan
terraform apply
```
7. **Deploy Super Mario on Kubernetes**
- Apply the deployment.yaml and service.yaml manifests:
```
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```
- Verify pod and service status:
```
kubectl get pods
kubectl get svc
```
---

**🎮 Accessing the Game**
Once the deployment is complete:
1. Retrieve the LoadBalancer URL or NodePort assigned to the service.
2. Open the URL in your browser — you’ll see Super Mario running on your Kubernetes cluster! 🕹️

**📁 Project Structure**
```
super-mario-k8s-deployment/
├── Dockerfile
├── deployment.yaml
├── service.yaml
├── README.md
└── screenshots/
    └── mario-ui.png
```
    
**📸 Screenshots**
Super Mario in Action
<img width="927" height="382" alt="image" src="https://github.com/user-attachments/assets/da31f3a8-1f11-477f-987b-192dd33124cb" />

## 🎥 Demo Video

https://github.com/user-attachments/assets/e553d0f2-7861-4792-9ef1-9f440b76d8ea

**📚 Learnings & Outcomes**
- Understanding of Terraform for provisioning cloud-native infrastructure.
- Hands-on experience with Kubernetes deployment and service management.
- Insight into end-to-end DevOps automation workflows.
- Practical understanding of Infrastructure as Code (IaC) and Container Orchestration.

**🧾 Future Enhancements**
- Integrate CI/CD pipelines using GitHub Actions or Jenkins.
- Implement auto-scaling based on traffic.
- Use Helm charts for more modular Kubernetes deployments.
- Add monitoring & logging with Prometheus and Grafana.

**🧑‍💻 Author**
**Kritika Aggarwal**
- 🎓 B.Tech Student, Bharati Vidyapeeth College of Engineering
- 💡 Passionate about Cloud, DevOps, and AI Technologies
- 🔗 LinkedIn Profile
---

**🌐 License**
- This project is open-source and available under the MIT License.
---

