# NETWORKWALKS_B084E_WK1_PM1_Lab_Setup

# Cybersecurity Lab Environment Setup

## Project Overview

This project focuses on setting up a basic cybersecurity testing lab using Oracle VirtualBox and Kali Linux. The lab provides a virtual environment for learning cybersecurity, penetration testing, network scanning, and ethical hacking.

## Objectives

- Install Oracle VirtualBox.
- Set up Kali Linux as the attacking machine.
- Configure a NAT Network using the `10.0.0.0/24` subnet.
- Assign the IP address `10.0.0.2/24` to Kali Linux.
- Enable Internet access for the Kali Linux virtual machine.
- Enable clipboard sharing and drag-and-drop functionality.
- Configure a shared folder between the host machine and Kali Linux.

## Tools and Technologies

- **Virtualization Software:** Oracle VirtualBox
- **Operating System:** Kali Linux
- **Network Type:** NAT Network
- **Subnet:** `10.0.0.0/24`
- **Kali Linux IP:** `10.0.0.2/24`

## Lab Configuration

| Component | Configuration |
|---|---|
| Host Operating System | Windows 10 |
| Virtualization Software | Oracle VirtualBox |
| Attacking Machine | Kali Linux |
| Network Type | NAT Network |
| Network Address | `10.0.0.0/24` |
| Kali Linux IP Address | `10.0.0.2/24` |
| Default Gateway | `10.0.0.1` |
| Internet Access | Enabled |
| Shared Folder | `/downloads` |
| Clipboard Sharing | Enabled |
| Drag and Drop | Enabled |

## Setup Procedure

### Step 1: Install VirtualBox

Download and install Oracle VirtualBox on the host machine.

### Step 2: Set Up Kali Linux

Download the Kali Linux virtual machine and import it into VirtualBox. Configure the virtual machine with the required system resources.
<img width="1920" height="1044" alt="Kali VM Setup" src="https://github.com/user-attachments/assets/c17b41eb-e630-42a9-b36b-40f5b8c51ec7" />

### Step 3: Configure the NAT Network

Create a NAT Network in VirtualBox with the following configuration:

- Network Name: `NatNetwork`
- IPv4 Prefix: `10.0.0.0/24`
- Network Type: NAT Network

Connect the Kali Linux virtual machine to this network.
<img width="1920" height="1043" alt="Network Settings" src="https://github.com/user-attachments/assets/094e4ddd-e3be-4269-abee-ad097b335dde" />

### Step 4: Configure the Kali Linux IP Address

Configure the network interface of Kali Linux with the following settings:

- IP Address: `10.0.0.2`
- Subnet Mask: `255.255.255.0`
- Default Gateway: `10.0.0.1`
- DNS Server: `8.8.8.8`
<img width="1920" height="1042" alt="Kali Network Settings" src="https://github.com/user-attachments/assets/7cd24a26-e73b-4bff-a2d0-c79693a57ce3" />

### Step 5: Enable Shared Features

Configure the VirtualBox settings to enable:

- Shared Clipboard: Bidirectional
- Drag and Drop: Bidirectional
- Shared Folder: `/downloads`
<img width="1920" height="1044" alt="Shared_Folder" src="https://github.com/user-attachments/assets/9508a816-4990-475b-a5e0-fb73fcda6b64" />

These features help transfer files and text between the host machine and the virtual machine.

### Step 6: Verify the Configuration

Run the following commands in Kali Linux to verify the network configuration and connectivity.

Check the IP address:

```bash
ip a
```

Test connectivity with the gateway:

```bash
ping 10.0.0.1
```

Test Internet connectivity:

```bash
ping 8.8.8.8
```

Test DNS resolution:

```bash
nslookup google.com
```

## Challenges Faced

No major problems were encountered during the lab setup. The required virtual machine and network configuration were completed successfully.

## What I Learned

Through this project, I learned:

- How to set up a virtual machine using VirtualBox.
- How to configure Kali Linux for cybersecurity practice.
- The basics of NAT Network and IPv4 addressing.
- How to configure network settings, gateways, and DNS.
- How to enable shared folders, clipboard sharing, and drag-and-drop functionality.
- How to verify network and Internet connectivity.

## Security and Ethical Use

This lab is intended for educational purposes and authorized cybersecurity testing only. Any testing activities should be performed on systems that I own or have explicit permission to test.

## Tools and Resources

- **Oracle VirtualBox:** https://www.virtualbox.org/wiki/Downloads
- **Kali Linux:** https://www.kali.org/get-kali/

## Author

**Atharv Shinde**

GitHub: https://github.com/LuciFer-1309

Linkedin: https://www.linkedin.com/in/atharv-shinde-724906390/

