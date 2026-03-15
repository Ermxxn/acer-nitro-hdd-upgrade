# Acer Nitro 5 (AN515-57) Storage Upgrade 🛠️

A step-by-step documentation of a hardware storage upgrade on an Acer Nitro 5 gaming laptop. This project demonstrates practical hardware handling, system disassembly, component installation, and software-level disk initialization.

## 📋 Project Overview
* **Device:** Acer Nitro 5 (AN515-57)
* **Component Installed:** 512GB Seagate 2.5" HDD
* **Objective:** Safely expand internal storage capacity while maintaining system integrity and testing post-installation performance.

## 🧰 Tools & Components
* Seagate 512GB 2.5" Hard Disk Drive
* Acer HDD Upgrade Cable (Proprietary SATA connector)
* Precision Screwdriver Set
* Plastic Prying Tools (Spudger/Picks)
* Anti-static mat/surface

![Tools and Preparation](images/1000159502.jpg)

---

## ⚙️ Installation Process

### 1. Chassis Disassembly
Carefully removed the bottom casing screws and used a plastic prying tool to detach the back cover without damaging the retention clips.

![Back Cover Intact](images/1000159504.jpg)
![Internals Exposed](images/1000159505.jpg)

### 2. Component Preparation
Prepared the empty 2.5" drive bay by removing the aluminum mounting caddy. 

![Empty Drive Bay](images/1000159514.jpg)

### 3. HDD Mounting and Cable Routing
Mounted the Seagate HDD into the caddy and secured it back into the chassis. Connected the proprietary Acer HDD upgrade cable to the drive.

![HDD Caddy Installed](images/1000159513.jpg)
![HDD Cable Close-up](images/1000159499.jpg)

### 4. Motherboard Connection
Delicately routed the SATA ribbon cable and seated the connector into the motherboard's HDD port, ensuring the locking mechanism was fully secured to prevent data corruption from a loose connection.

![Motherboard Connection](images/1000159507.jpg)

### 5. Reassembly
Reattached the bottom chassis, ensuring all clips snapped back into place and all screws were re-seated firmly.

![Reassembled Laptop](images/1000159518.jpg)

---

## 💻 System Configuration & Benchmarking

After physically installing the drive, the system required software-level configuration to recognize and utilize the new hardware.

### Disk Initialization
Booted into Windows and used **Disk Management** to initialize the new disk, allocate the unallocated space, and format it as a New Simple Volume (NTFS). The system successfully recognized the drive as "HardDisk (D:)" with 465.76 GB of usable space.

![Disk Management Initialization](images/1000159519.jpg)

### Performance Testing
Ran a command-line storage assessment using the Windows System Assessment Tool (`winsat`). 
* **Command used:** `winsat disk -drive d`
* Verified standard mechanical drive read/write speeds, confirming the SATA connection was stable and functioning optimally.

![Winsat Benchmark](images/1000159537.jpg)

---
*Documented for portfolio purposes to demonstrate practical hardware integration and system management.*
