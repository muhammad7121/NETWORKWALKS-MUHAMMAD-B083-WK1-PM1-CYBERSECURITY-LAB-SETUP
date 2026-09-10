# NETWORKWALKS-MUHAMMAD-B083-WK1-PM1-CYBERSECURITY-LAB-SETUP
    # Cybersecurity Lab Setup Using VirtualBox and Kali Linux

    ## Project Description

This project documents the process of setting up a personal cybersecurity laboratory using **Oracle VirtualBox and Kali Linux**. It covers the tools used, the steps taken to configure the virtual environment and network, as well as the challenges I encountered during the setup and how I resolved them.

    ## Objective

The main objective of this project was to:

* Set up a functional cybersecurity laboratory using Kali Linux.
* Learn how to install and configure a virtual machine using Oracle VirtualBox.
* Configure a virtual network using **NAT Network**.
* Assign and configure IP addresses manually.
* Test network connectivity between the Kali Linux environment and the internet.
* Develop practical skills in Linux, networking, virtualization, and cybersecurity.
* Create a safe environment for practicing cybersecurity tools and techniques.

      ## Tools Used

* **Windows** – Host operating system
* **Oracle VirtualBox** – Virtualization platform
* **Kali Linux** – Cybersecurity-focused Linux distribution
* **7-Zip** – Used to extract downloaded files
* **Kali Linux VirtualBox Image** – Used to create the Kali Linux virtual machine
* **Terminal** – Used to test network connectivity
* **Google DNS (8.8.8.8)** – Used for DNS configuration and connectivity testing

      ## Steps Taken

### Step 1: Downloading and Installing VirtualBox

I first used the link provided in **Week 1 (WK1)** to download **7-Zip**, which I used to extract the downloaded files. After that, I downloaded **Oracle VirtualBox**, extracted the necessary files, and installed VirtualBox on my Windows computer.

### Step 2: Configuring the Network

I configured the VirtualBox network to use **NAT Network**. I set the network address to **10.0.0.0/24** and enabled the **DHCP Server**. After making the necessary changes, I clicked **Apply** to save the configuration.

### Step 3: Downloading and Setting Up Kali Linux

I used the link provided in the PDF to download Kali Linux. Initially, I downloaded the **ISO file** and attempted to install it on VirtualBox, but the installation was not working.

I reached out to one of the team leads, **Muhammad Muhammad**, who assisted me and showed me the appropriate Kali Linux version to download for VirtualBox.

I deleted the previous setup and the ISO file and downloaded the **Kali Linux VirtualBox image** instead. After extracting the downloaded file, I opened it, and Kali Linux started running directly in VirtualBox.

### Step 4: Configuring Kali Linux Network Settings

I configured the network settings for Kali Linux by navigating to the network settings and changing **Attached to** to **NAT Network**. I selected the configured NAT Network and changed the permission to **Allow All**. I then clicked **OK** to save the settings.

### Step 5: Configuring a Static IP Address

I navigated to **Wired Connection 1**, right-clicked on it, and selected **Edit Connection**. I clicked **Add** and changed the connection method to **Manual**.

I initially configured:

* IP Address: **10.0.0.2**
* Netmask: **24**
* Gateway: **10.0.0.1**
* DNS: **8.8.8.8**

However, the network was not connecting successfully. I contacted **Muhammad Muhammad** again for assistance. He advised me to add another IP address:

* IP Address: **10.0.0.3**
* Netmask: **24**
* Gateway: **10.0.0.1**

He also asked me to ping **8.8.8.8** from the Kali Linux terminal to confirm that the system could communicate with the internet. After adding the new IP address and performing the ping test, the network connection was successfully established.

### Step 6: Checking the Kali Linux Configuration

I went back to the **Devices** section on my Kali Linux system and checked the available settings. I confirmed that the necessary options were enabled and properly configured.

I also checked the **Acceleration** settings and confirmed that everything was working correctly. Finally, I checked the **Shared Folder** settings to ensure that the configuration was properly set up.

     ## Challenges Encountered

During the setup, I encountered the following challenges:

1. **Network connectivity issue:**
   After configuring the static IP address, the network was not connecting as expected.

2. **Troubleshooting the network:**
   With assistance from the team lead, I added another IP address and tested the connection by pinging **8.8.8.8**, which helped confirm that the network was working.

           ## Lessons Learned

Through this project, I gained practical experience in:

* Setting up a virtual machine with VirtualBox.
* Installing and running Kali Linux.
* Configuring a NAT Network.
* Understanding IP addresses, netmasks, gateways, and DNS.
* Configuring a static IP address.
* Testing network connectivity using the `ping` command.
* Troubleshooting virtualization and network-related problems.
* Using guidance and troubleshooting steps to resolve technical issues.
* Preparing a controlled environment for cybersecurity practice.

      ## Conclusion

The cybersecurity laboratory was successfully set up using **Oracle VirtualBox and Kali Linux**. Although I encountered challenges during the Kali Linux installation and network configuration, I was able to resolve them with troubleshooting and guidance from the team lead. The completed lab provides a practical environment for continuing my learning and developing hands-on cybersecurity skills.
