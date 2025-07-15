# 🚀 Automated CI/CD Pipeline with Jenkins and Ansible

This project demonstrates a complete **CI/CD pipeline** using **Jenkins (Declarative Pipeline)**, **Ansible**, and **GitHub**, deploying a sample web application to a remote **AWS EC2 app server** using Apache2.

---

## 🔧 Technologies Used

- 🟠 Git & GitHub
- 🟢 Jenkins (Declarative Pipeline)
- 🔵 Ansible
- ☁️ AWS EC2 (Jenkins server + App server)
- 🌐 Apache2 Web Server (on App Server)

---

## 📁 Project Structure

sample-web-app/
├── index.html # Sample web page
├── deploy.yml # Ansible playbook to deploy web app
├── hosts.ini # Inventory file for app server
└── Jenkinsfile # Jenkins declarative pipeline script


---

## 🛠️ Jenkins Pipeline Flow

1. Developer pushes code to GitHub (`main` branch)
2. Jenkins Pipeline is triggered manually (can add webhook later)
3. Jenkins checks out code via `Jenkinsfile`
4. Jenkins executes Ansible playbook
5. Web page is deployed to remote EC2 app server
6. Apache2 serves the HTML file publicly

---

## 🔐 Security & SSH Setup

- SSH key-based authentication setup between Jenkins server and App server
- Private key stored in Jenkins home `.ssh` for automation
- Ansible connects over SSH from Jenkins agent to App server

---

## 🌐 Live Output

> Visit: [http://54.242.26.56](http://54.242.26.56)

You will see:
Welcome to My Website – Deployed via Jenkins CI/CD!


---

## 🧠 What I Learned

- Configuring Jenkins Pipeline from SCM (GitHub)
- Writing `Jenkinsfile` using declarative syntax
- Executing Ansible playbooks from Jenkins
- Secure SSH deployment setup
- Apache2 hosting on Ubuntu EC2 instance
- Managing inventory and playbooks in GitHub

---

## 🏁 Result

✅ A fully automated CI/CD pipeline powered by Jenkins + Ansible  
✅ No manual server login or file copying  
✅ Easily extendable for Docker, Webhooks, or Multi-Stage apps

---

📘 **Project by:** Praveen Patnala  
📆 **Completed:** July 2025  

