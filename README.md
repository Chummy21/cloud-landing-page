# The Future of AI-Powered Trading Technology

### NAME: Chioma Okafor
### ALTSCHOOL ID:ALT/SOE/024/4939

---

# 🌥️ 
## 📌 Project Description

This project showcases a responsive cloud-themed landing page, deployed on an AWS EC2 instance with Nginx as the web server. It was developed as part of my 
AltSchool Africa Tinyuka Second Semester coursework, where I explored the core principles of Linux server provisioning, static site deployment, and web server 
configuration in a real-world cloud environment.



## 🔗 Live Demo

Access the deployed site via the Public IP:  
👉 [http://18.169.190.77](http://18.169.190.77)


## 🗂️ Project Structure

ai-cloud-landing-page/
├── index.html
├── style.css
├── README.md

## 📌 Features

- Responsive HTML/CSS landing page
- Tailwind CSS for styling via CDN
- Hosted on AWS EC2 Ubuntu server
- Nginx web server for deployment
- Git + GitHub for version control
- FreeDNS subdomain mapping (optional)
- Optional reverse proxy and SSL via Let’s Encrypt (Certbot)


## 🚀 Steps Taken

### 1. 🖊️ Created the Web Page
- Built a basic HTML + CSS landing page
- Added Tailwind CSS via CDN to enhance styling and responsiveness

### 2. 📁 Pushed to GitHub
- Initialized a Git repo locally
- Connected to a GitHub repo
- Used `git push` to upload files

### 3. 💻 Provisioned EC2 Server
- I created a new Ubuntu EC2 instance on AWS Provisioning the Server
- Cloud Provider: Amazon Web Services (AWS)
- Service Used: EC2 (Elastic Compute Cloud)
- Instance Type: t2.micro (free-tier eligible)
- Operating System: Ubuntu Server 22.04 LTS (64-bit)
- Storage: 8 GB General Purpose SSD
- Set up security groups to allow:
  - HTTP (port 80)
  - HTTPS (port 443)
  - SSH (port 22)

### EC2 Instance Showing Ubuntu OS
![EC2 Instance Showing Ubuntu OS](./assets/UbuntuOS.png)

### EC2 Instance Showing Ubuntu OS
![EC2 Instance Showing Public IP](./assets/public IP and Ubuntu OS.png)


### 4. Web Server: Nginx
- Tools Installation:
  - sudo apt update
  - sudo apt install nginx git -y
- Configuration:
  - Updated /etc/nginx/sites-available/default to serve the HTML landing page.
  - Used systemctl to restart and enable Nginx.
- Deployment Directory: /var/www/html
  - Bonus: Configured a reverse proxy (optional setup, attempted but not using Node.js).

### 5. Cloned the GitHub Repo on EC2 Using:
 - git clone https://github.com/Chummy21/ai-cloud-landing-page.git

### 6. Deployed the Files
 - sudo cp -r ai-cloud-landing-page/* /var/www/html/

### 7. 🌍 Connected a Subdomain (Optional)
 - Registered a subdomain on FreeDNS
 - Pointed it to my EC2 Public IP
 - verified using ping and browser

### 8. 🛡️ Secured with SSL (Optional)
 - Used Certbot to install Let's Encrypt SSL (only if the domain was active):
  - sudo apt install certbot python3-certbot-nginx -y
  - sudo certbot --nginx

### 9. 🎨 Tailwind CSS
 - Tailwind was added using CDN in index.html:
  - <script src="https://cdn.tailwindcss.com"></script>
   - I also Used utility classes like:
     - <div class="bg-blue-500 text-white text-center p-4"

