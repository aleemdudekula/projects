# DevOps Learning Projects 🚀

This repository documents my hands-on journey learning DevOps tools and cloud infrastructure.
Instead of only watching tutorials, I focus on **building, deploying, and troubleshooting real systems**.

---

## 📚 Topics Covered

* Linux server basics
* Git and GitHub workflows
* AWS EC2 cloud infrastructure
* Nginx web server configuration
* Static website deployment
* SSH authentication and key management
* Networking and security groups

---

## ⚙️ Project 1 — Deploying a Static Website on AWS EC2

### Objective

Deploy a static HTML website from a Git repository to an AWS EC2 instance and serve it using **Nginx**.

### Architecture

Local Machine → GitHub Repository → AWS EC2 → Nginx → Public Website

---

### Step 1 — Launch EC2 Instance

* Created an EC2 instance (Ubuntu)
* Generated and downloaded SSH key pair
* Configured Security Group rules

Ports opened:

| Port | Purpose             |
| ---- | ------------------- |
| 22   | SSH access          |
| 80   | HTTP website access |

---

### Step 2 — Connect to the Server

```bash
ssh -i key.pem ubuntu@EC2_PUBLIC_IP
```

---

### Step 3 — Install Nginx

```bash
sudo apt update
sudo apt install nginx
```

Check service status:

```bash
sudo systemctl status nginx
```

---

### Step 4 — Deploy Website Files

Clone repository or copy website files into the Nginx web root directory:

```bash
sudo cp -r project-folder/* /var/www/html/
```

---

### Step 5 — Restart Nginx

```bash
sudo systemctl restart nginx
```

---

### Step 6 — Access the Website

Open in browser:

```
http://EC2_PUBLIC_IP
```

The website is now live from the EC2 server.

---

## 🧠 Key Concepts Learned

* Difference between **public IP and private IP**
* How **Nginx serves static files**
* How **AWS security groups control traffic**
* Using **SSH keys for authentication**
* Linux file permissions and server directories

---

## 🤝 Connect

I'm documenting my DevOps learning journey publicly.
Feel free to explore the repository or suggest improvements.

LinkedIn: https://www.linkedin.com/in/aleem-dudekula-99b95525b/

