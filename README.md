# THE LOVERS 

In this lab, you will exploit a classic SQL Injection vulnerability to access the admin panel of a dating app. From there, you will obtain sensitive credentials and progress to uncover hidden relationships, secret directories, and privileged users. In this lab, you will learn:

- Identification and exploitation of SQL Injection in login forms
- Remote access to Linux servers via SSH
- Searching for sensitive information in user profiles
- Cracking hashes with tools like `hashcat`
- Privilege escalation based on users with root permissions

<how-to-start>
   
## 🌱 How to start this lab

Follow these instructions to get started:

1. **Download the virtual machine** from this [link](https://storage.googleapis.com/cybersecurity-machines/lovers-lab.ova).
2. **Import the machine** into your preferred virtualization manager (VirtualBox, VMware, etc.).
3. Once the machine is running, you can start the lab!

</how-to-start>


## 📄 Instructions

You are facing a romantic and vulnerable web application. Your mission is to use your technical skills to uncover the secrets behind this panel.

1. **Discover the IP address of the THE LOVERS machine.**
   - Use tools like `nmap`, `netdiscover`, or `arp-scan` to scan the network.

2. **Access the website hosted on the server.**: You will find a landing page with a typical dating app login. Use SQL Injection to log in without real credentials.

3. **Access the admin panel of the user Mike.**

4. **Connect to the server via SSH as Mike.**

5. **Find the first flag.**

6. **Explore the `secrets` directory.**

7. **Discover Amanda's password and switch users.**

8. **Access the final flag as root.**

**Remember:** even secret loves leave digital traces. 💔

Good luck!