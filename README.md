What it is: A small web app deployed using EC2 for compute, S3 for storage, IAM for permissions, Cloudwatch for monitoring

Why it exists: Learn to deploy, secure, and monitor a functioning AWS system

Setup/Usage: (Add this later, once runnable.)

Next steps: connect and configure, Add S3 storage, Secure with IAM, Monitor & clean up

<img width="1366" height="720" alt="image" src="https://github.com/user-attachments/assets/9f212554-4375-465f-aaf7-f7f74f7ad6da" />


## AWS EC2 Webpage Demo 🚀

This project demonstrates deploying a simple static HTML webpage on an **AWS EC2 instance**, covering the essentials of cloud server setup, SSH access, and web hosting.

### Live Demo Screenshot
<img width="1366" height="720" alt="image" src="https://github.com/user-attachments/assets/d70e0567-d8af-4e62-812e-881638f2a790" />

### Key Steps

1. **Launch an EC2 Instance**  
   - Used **Amazon Linux AMI**.

2. **Connect via SSH**  
   - From **Git Bash** on Windows:
   ```bash
   ssh -i "worker_server.pem" ec2-user@18.217.67.251

Deploy Webpage

echo '<h1>Hello from AWS EC2!</h1>' | sudo tee /var/www/html/index.html

Start Apache Web Server

sudo systemctl start httpd
sudo systemctl enable httpd

Configure Security Group

Allow HTTP (port 80) traffic from your IP or temporarily 0.0.0.0/0 for testing.

View Webpage

Navigate to EC2 public IP in a browser to see the live page.

Notes:

This is a learning project intended to practice AWS cloud and web hosting fundamentals.

Next steps: Add S3 storage, Secure with IAM, Monitor & clean up
