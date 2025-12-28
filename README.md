
# Networking Assignment

## Core Assignment: Domain + EC2 + DNS NGINX


## Objective
- Register a domain
- Launch an EC2 instance
- configure to correct security group
- Install and run NGINX
- Configure DNS (A record) to point the domain to the EC2 public IPv4 address
- Confirm the site loads in a browser

### 1. Registering a domain

I went to AWS Route 53 and registered a domain.

<img src="images/buy-domain.png" width="600" alt="Route 53 domain registration">

**Domain:** `libanisse.co.uk`
**Website:** https://www.libanisse.co.uk

### 2. Launch an EC2 instance + connect with SSH

Next, I launched an EC2 instance (Ubuntu) and created a new key pair so I could securely connect to the server.

<img src="images/connect-ec2.png" width="600" alt="EC2 instance running and SSH connection">

### Commands used for NGINX
- sudo apt update
- sudo apt install -y nginx

- sudo systemctl start nginx
- sudo systemctl enable nginx

- sudo systemctl status nginx --no-pager

<img src="images/nginx-status.png" width="450" alt="nginx update and status">

### 3. Elastic IP

I allocated and associated an Elastic IP with my EC2 instance so the server keeps the same public IP address.

<img src="images/elastic-ip.png" width="600" alt="Elastic IP associated with EC2 instance">

