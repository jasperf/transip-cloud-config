# transip-cloud-config

This repository contains a cloud-config file designed for automating server configuration in a cloud environment. Key features include:

User account setup for transip with pre-configured SSH access using an SSH public key.
Secure SSH configuration with root login disabled and password authentication turned off.
Custom SSH port configuration (Port 12345) for enhanced security.
Automated creation and modification of SSH configurations (/etc/ssh/sshd_config).
Installation of essential packages and post-install callbacks for monitoring provisioning.
This cloud-config is suitable for quickly setting up Ubuntu-based cloud servers with enhanced security practices, ensuring consistent and repeatable server provisioning.










