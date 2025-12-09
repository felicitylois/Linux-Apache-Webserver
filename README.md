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
<img width="1938" height="1454" alt="01_Update System Packages" src="https://github.com/user-attachments/assets/793cd515-2258-4670-9492-1d2d764eaf39" />


### 2️⃣ Install Apache Web Server
**Installed Apache using the package manager**
```shell
sudo apt install apache2 -y
```
<img width="1953" height="1464" alt="01_Install_Apache_Web_Server" src="https://github.com/user-attachments/assets/02ab5a15-623c-4921-98aa-fd007bda7cb2" />

**Check service status**
```shell
sudo systemctl status apache2
```
<img width="1938" height="1505" alt="Verify_service_status" src="https://github.com/user-attachments/assets/600ad265-86f9-47b7-8684-fe12ac031d58" />

### 3️⃣ Manage Apache as a System Service
I managed Apache using systemctl to start, stop, restart, and enable it on boot, ensuring the web server would always be available when the system started
```shell
sudo systemctl start apache2
sudo systemctl stop apache2
sudo systemctl restart apache2
sudo systemctl enable apache2
```
<img width="2880" height="1800" alt="03_Manage_Apache_as_a_System Service" src="https://github.com/user-attachments/assets/b60320d5-a301-40a6-ace3-ca125d52bd67" />


### 4️⃣ Configure and Secure the Server with UFW Firewall
I secured the server using UFW, allowing only HTTP and HTTPS traffic to reduce the attack surface and prevent unauthorized access:
<img width="971" height="768" alt="4_Configure_and_Secure_the Server_with_UFW_Firewall" src="https://github.com/user-attachments/assets/460bc4d1-4836-4d92-9dcf-a156be89e969" />

### 5️⃣ Verify Apache Is Working
I confirmed the Apache web server was operational by opening a browser and visiting `http://localhost`, ensuring the default page loaded correctly.
<img width="1372" height="866" alt="Verify_Apache_Is_Working" src="https://github.com/user-attachments/assets/84b5c569-9941-471d-adc6-d987637176f3" />

### 6️⃣ Check Network Configuration
I used `ip a` to identify the server’s IP address and tested access from another device on the same network to verify external connectivity
<img width="962" height="475" alt=" 06_Check_Network_Configuration" src="https://github.com/user-attachments/assets/f604d93a-be2e-4d33-bc01-10162b83a85f" />

### 🛠 Tools Used
- Ubuntu
- apache2
- bash
- apt
- systemctl
- ip
