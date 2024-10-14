# Cloud-Config for Server Setup Automation

This repository contains a cloud-config file that automates server configuration in a cloud environment. The configuration is tailored for Ubuntu-based servers and includes the following features:

### Key Features

- **User and Group Setup**:
  - Creates a user account named `transip` with predefined groups and SSH access.
  - Adds your public SSH key for secure, password-less authentication.

- **SSH Configuration**:
  - Disables root login and password authentication for increased security.
  - Configures SSH to use a custom port (`Port 12345`).
  - Automatically updates `/etc/ssh/sshd_config` to apply the new SSH settings.

- **Package Installation**:
  - Installs predefined packages (`packagename1`, `packagename2`).

- **System Security**:
  - Ensures that only authorized users can access the server, enhancing overall security.

- **Custom Post-Installation Callback**:
  - Uses the `phone_home` feature to notify a specified URL upon successful installation.

### How to Use

1. Save the cloud-config file as `cloud-config.yaml`.
2. Deploy it using your cloud provider's instance creation options.
3. Modify any settings, such as the SSH port or authorized keys, as needed.

### TransIP Documentation
For more information on using cloud-config with TransIP, refer to their [knowledge base](https://www.transip.eu/knowledgebase/3424-how-use-cloud-config-file/).

### Notes
- Ensure you replace `your password` in the `chpasswd` section with a secure root password.
- Adjust package names as required for your use case.

This configuration is ideal for consistent and secure server deployments, reducing manual setup effort and enforcing best practices.

