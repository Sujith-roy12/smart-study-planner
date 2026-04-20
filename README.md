# 🚀 Smart Study Planner (Cloud SaaS Edition)

A fully front-end, zero-dependency task management and focus system built for the Cloud Computing Lab Evaluation. This application demonstrates a "Software as a Service" (SaaS) model and is designed to be easily deployed on Platform as a Service (PaaS) like Vercel and Infrastructure as a Service (IaaS) like AWS EC2.

![Smart Study Planner Banner](https://via.placeholder.com/800x400.png?text=Smart+Study+Planner+%7C+Cyberpunk+SaaS)

## ✨ 5 Core Features

1. **Task Management System:** Add study tasks with subjects, topics, and time estimates.
2. **Priority Tagging:** Assign High, Medium, or Low priorities to automatically sort the task queue.
3. **Progress Tracking:** A real-time dashboard calculating completion percentage and remaining tasks.
4. **Smart Suggestion Engine:** Dynamic alerts that analyze the task list to warn about pending High-priority tasks or suggest entering Focus Mode.
5. **Fullscreen Integrity Focus:** A lock-down Pomodoro timer that takes over the screen. It tracks "Integrity Violations" by monitoring tab activity (`window.onblur`), forcefully consuming a "Break" token if the user attempts to browse other sites without authorization.

## 🛠️ Tech Stack
- **Structure:** Pure HTML5
- **Styling:** CSS3 (Grid, Flexbox, Custom Cyberpunk Terminal Aesthetics)
- **Logic:** Vanilla JavaScript (ES6, LocalStorage for persistence)
- **Zero Dependencies:** No frameworks required, making it incredibly lightweight and robust.

## ☁️ Cloud Deployment Integrations

### 1. PaaS Deployment (Vercel/Netlify)
This architecture is entirely client-side, making it perfect for instantaneous static hosting.
1. Upload this repository to your GitHub account.
2. Sign in to [Vercel](https://vercel.com).
3. Click "Add New Project" and import this repository.
4. Click **Deploy**. Vercel instantly handles the SSL, CDN, and hosting.

### 2. IaaS Deployment (AWS EC2)
To prove infrastructural control, this app can be manually hosted on a raw EC2 server.
1. Launch an Ubuntu EC2 instance on AWS.
2. Ensure **Port 80 (HTTP)** traffic is allowed in your Security Group.
3. Connect via SSH:
   ```bash
   ssh -i "your-key.pem" ubuntu@<your-ec2-ip>
   ```
4. Install the Apache web server:
   ```bash
   sudo apt update
   sudo apt install apache2 -y
   ```
5. Replace the default `/var/www/html/index.html` with the `index.html` file in this repository.

## 🔒 Local Installation
Simply download this repository and double click `index.html`. No backend setup or terminal commands required! The application uses local browser storage to save your tasks persistently on your machine.
