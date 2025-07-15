# Automated CI/CD Pipeline with Jenkins and Ansible 🚀

This project demonstrates a complete CI/CD pipeline using **Jenkins**, **Ansible**, and **GitHub**, deploying a sample web application to an **AWS EC2 app server**.

## 🔧 Technologies Used
- Git & GitHub
- Jenkins
- Ansible
- AWS EC2 (Jenkins server + App server)
- Apache2 Web Server

## 📁 Project Structure
├── index.html # Sample web page
├── deploy.yml # Ansible playbook to deploy HTML to app server
├── hosts.ini # Ansible inventory file


## 📦 How It Works
1. Code pushed to GitHub
2. Jenkins Freestyle Job pulls the repo
3. Ansible Playbook runs from Jenkins server
4. Web page deployed to remote EC2 App server via SSH
5. Apache2 serves the page at `http://<app-server-ip>`

## 🌐 Live Test
http://54.242.26.56

## 🏁 Result
On successful build, the app server displays:
> "Welcome to My Website – Deployed via Jenkins CI/CD!"

