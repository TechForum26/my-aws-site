# EC2 Static Website Project

A simple HTML + CSS + JS website deployed on an AWS EC2 instance using Apache and Git.

---

## Aim of the Project

- Hosting a static website on EC2
- Using Git (with SSH or token) to push/pull from GitHub
- Setting up Apache server
- Updating content using Git

---

## Files to be included 

- `index.html` – Static webpage
- `script.sh` – Optional script to automate deployment steps

---

## Deployment Steps on EC2

1. **Install Apache**

sudo apt update
sudo apt install apache2

2. **Allow port 80 (in AWS Security Group)**
3. **Clone the GitHub repo**

git clone https://github.com/YourUsername/your-repo.git

4. **Move files to Apache web root**

sudo cp your-repo/index.html /var/www/html/

5. **Start Apache**

sudo systemctl start apache2

6. **Open your EC2 public IP in a browser**

http://<your-ec2-ip>

