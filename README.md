# Remote Server Creation Tutorial 
This tutorial will explain how you can create a remote server through a Linux Virtual Machine (VM) using Digital Ocean, a cloud service provider. 

In this tutorial, you will learn how to: 
- **Create SSH keys on your local machine**
- **Use the web console to add a custom Arch Linux image**
- **Create a Droplet**
- **Use a cloud-init configuration file**
- **Use your SSH keys to connect to your server.**

# Requirements
- A computer with Windows OS 
- Access to Windows Powershell 
- Command-line input knowledge 
- A Digital Ocean Account 

# Create an SSH Key 
Before we get started, you may be wondering what SSH means and what an SSH key is. SSH stands for Secure Shell and it is a security protocol that manages communication between a device and a "unsecured network" (Cloudflare). In this case, the SSH protocol is managing the communication between a computer and a remote server. When data is sent between the computer and the remote server, SSH will use "encryption"(Cloudflare) to make the data unreadable to any outside party that's not involved between the connection. 

An SSH key involves a two-way process. It has a public key that is accessible to anyone and a private key that's only accessible by the key owner. This means you can access the server with or without a password as long as you have the key. Since the SSH will always have two keys, it is also called an SSH key pair. Now, let's get started!

Step 1: Open Windows Powershell 

Step 2: In the command-line, copy and paste this path.
``` 
ssh-keygen -t ed25519 -f C:\Users\your-user-name\.ssh\something-key -C "youremail@email.com"
```

Step 3: Customize the path you copy/pasted
- Replace "your-user-name" with your Windows username
- Name your key. Change "something-key" into your desired name. Ex: "ocean-key"
- Replace "youremail@email.com" with your desired email address

Step 4: Press the "Enter" key. You will be asked to enter a passphrase or to leave it empty for no passphrase. You will then receive a confirmation message that your key has now been created. 






