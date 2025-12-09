# 🖥️ Linux Apache Webserver
In this project, I built and secured an Apache web server on a Debian-based Linux system, managing services, configuring a UFW firewall, and verifying network access to create a functional and secure web environment.

## 🎯 Project Highlights
- I installed Apache using APT and configured it to run reliably.
- I managed the Apache service with `systemctl` to start, stop, and enable it on boot.
- I secured the server by setting up a UFW firewall to allow only necessary traffic.
- I verified that the default web page loads on `http://localhost`
- I checked network configuration using `ip a` to ensure connectivity.
- I tested the server from another device to confirm it was functional and accessible.

## 📸 Screenshots
### 1️⃣ Update System Packages
```shell
sudo apt update && sudo apt upgrade -y
```

### 2️⃣ Install Apache Web Server
**Installed Apache using the package manager**
```shell
sudo apt install apache2 -y
```

**Check service status**
```shell
sudo systemctl status apache2
```

### 3️⃣ Manage Apache as a System Service
I managed Apache using systemctl to start, stop, restart, and enable it on boot, ensuring the web server would always be available when the system started

```shell
sudo systemctl start apache2
sudo systemctl stop apache2
sudo systemctl restart apache2
sudo systemctl enable apache2
```
### 4️⃣ Configure and Secure the Server with UFW Firewall
I secured the server using UFW, allowing only HTTP and HTTPS traffic to reduce the attack surface and prevent unauthorized access:

### 5️⃣ Verify Apache Is Working
I confirmed the Apache web server was operational by opening a browser and visiting `http://localhost`, ensuring the default page loaded correctly.

### 6️⃣ Check Network Configuration
I used `ip a` to identify the server’s IP address and tested access from another device on the same network to verify external connectivity:
