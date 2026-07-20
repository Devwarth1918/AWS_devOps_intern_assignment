# AWS_devOps_intern_assignment
Simple website deployment on AWS EC2 using Nginx.
## Name: Devwarth

## EC2 Setup Steps

1. Launched an Ubuntu EC2 instance.
2. Created a Security Group.
3. Allowed inbound rules:
   - Port 22 (SSH)
   - Port 80 (HTTP)
4. Connected to the EC2 instance using SSH.
5. Allocated and associated an Elastic IP.

---

## Nginx Installation

Update packages

```bash
sudo apt update
```

Install Nginx

```bash
sudo apt install nginx -y
```

Check Nginx status

```bash
sudo systemctl status nginx
```

Restart Nginx

```bash
sudo systemctl restart nginx
```

---

## Website Deployment

Created an `index.html` file and placed it in:

```text
/var/www/html/
```

Restarted Nginx and accessed the website using the Elastic IP.

---

## Commands Used

```bash
sudo apt update
sudo apt install nginx -y
sudo systemctl status nginx
sudo systemctl restart nginx
df -h
free -h
ps aux
chmod +x restart_nginx.sh
./restart_nginx.sh
```
