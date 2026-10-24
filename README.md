**SSH Server Hardening & Key Based Authentication Lab** 

**Overview**
This project demonstrates how I secured SSH access on an ubuntu linux system by creating a key based authentication and disabling insecure login methods.

**Objectives**
Configure and secure an OpenSSH server, Generate ED25519 key pair, Configure SSH public key authentication, Disable password based SSH authentication, Prevent direct root SSH login, Test authorized and unauthorized methods.

**Tools** 
Ubuntu Linux, OpenSSH Server, Linux Terminal, SSH Keygen, GitHub

**Implementation** 
1. SSH Server Setup - Install and verify the OpenSSH server
2. SSH Key Generation - Generated an ED25519 SSH key pair using ssh-keygen -t ed25519 -C "kingsley-ssh-lab"
3. Public Key Authentication - Installed the public key using ssh-copy-id and successfully authenticated to the local SSH server
4. SSH Security Configuration - Configured SSH server with PermitRootLogin no and PasswordAuthentication no. Validated the configuration and reloaded the SSH service
5. Security Testing - Successfully connected SSH key based authentication, Attempted password only SSH authentication, Confirmed the password only authentication was rejected with permission denied (pubickey)

**Results**
Successfully hardened SSH authentication by disabling password based access and direct root login while maintaining authorized access through SSH keys.

**Skills Demonstrated**
Linux System Administration, SSH Server Hardening, Public Key Crptography, Authentication Security, Access Control, Security Configuration Testing

**Lab Enviornment**
Testing was performed in Ubuntu Linux lab using local host (127.0.0.1).
