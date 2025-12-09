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
