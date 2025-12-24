# 🛡️ Linux Security Dashboard (Tkinter)

A **desktop-based Linux Security Dashboard** built with **Python + Tkinter**, designed to provide multiple system security and monitoring utilities in a single graphical interface.

This project integrates file integrity monitoring, system resource tracking, network activity inspection, password security tools, encryption utilities, firewall management, and USB device monitoring.

---

## 📌 Features Overview

### 🔐 File Integrity Monitor

* Select files to monitor for unauthorized changes
* Uses **SHA-256 checksums**
* Detects modifications and logs timestamps
* Real-time alerts on file tampering

---

### 📊 Resource Monitor

* Live CPU usage graph
* Live RAM usage graph
* Uses **psutil + matplotlib**
* Auto-updating every second

---

### 🌐 Network Monitor

* Displays active network connections
* Shows protocol, local/remote address, status, and PID
* Real-time **network traffic graph** (KB/s sent & received)
* Useful for spotting suspicious activity

---

### 🔑 Password Strength Checker

* Checks password strength using:

  * Length
  * Uppercase / lowercase
  * Digits
  * Special characters
* Generates strong random passwords
* One-click copy to clipboard

---

### 🔐 Encryption & Decryption Tool

* Uses **Fernet symmetric encryption**
* Generate secure encryption keys
* Encrypt and decrypt messages
* Clipboard support for keys and encrypted data

---

### 🚫 Firewall Rule Manager

* Add firewall rules using **iptables**
* Block IPs or IP + port
* Remove firewall rules
* List current blocked IPs
* Built-in **NSLookup tool**
* Block domains by resolving and blocking all IPs

> ⚠️ Requires **sudo privileges**

---

### 🔌 USB Device Monitor

* Lists all connected USB devices
* Shows Bus, Device ID, Vendor/Product details
* Displays extended device info using `udevadm`
* Real-time detection of USB plug/unplug events

---

## 🧰 Tech Stack

* **Python 3**
* **Tkinter / ttk**
* **psutil**
* **matplotlib**
* **seaborn**
* **cryptography (Fernet)**
* **pyudev**
* **iptables / ipset**
* **lsusb / udevadm**

---

## 📂 Project Structure

```
Linux-Security-Dashboard/
│
├── main.py              # Main application (all modules)
├── README.md            # Project documentation
└── requirements.txt     # Python dependencies
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/linux-security-dashboard.git
cd linux-security-dashboard
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ System Requirements (Linux)

```bash
sudo pacman -S iptables ipset usbutils udev   # Arch-based
# or
sudo apt install iptables ipset usbutils udev # Debian-based
```

---

## ▶️ Run the Application

```bash
sudo python main.py
```

> **Sudo is required** for firewall control, network inspection, and USB monitoring.

---

## 🔐 Permissions & Security Notes

* Firewall and network features require **root access**
* USB monitoring relies on **udev events**
* File Integrity Monitoring only tracks selected files
* Encryption keys are not stored automatically

---

## 🎓 Academic Use

This project is suitable for:

* Linux Security coursework
* System Programming labs
* Cybersecurity demonstrations
* Portfolio showcase projects

---

## 📜 License

This project is for **educational purposes**.
Use responsibly. Don’t block your university Wi-Fi unless you enjoy meetings.

