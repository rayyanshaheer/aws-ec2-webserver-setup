# Rayyan AWS Webserver Project

This is a personal project demonstrating **AWS EC2**, **NGINX**, and **PHP** setup.

## Overview

- Launched an **EC2 instance** (t2.micro) on AWS.
- Installed **NGINX** and **PHP-FPM**.
- Deployed a simple PHP page to test the web server.
- Explored **instance types and pricing** on AWS.

## Screenshots

- `aws-ec2_dashboard.png` – EC2 instance running.
- `aws-ssh_terminal.png` – Commands executed in SSH.
- `aws-php_page.png` – PHP page output in browser.
- `aws-instance_type.png` – Instance type & pricing info.

## Commands Used

```bash
sudo apt update
sudo apt install -y nginx php-fpm
sudo systemctl enable nginx
sudo systemctl start nginx
echo "<?php echo 'Hello from Rayyan'; ?>" | sudo tee /var/www/html/index.php
sudo chown -R www-data:www-data /var/www/html
