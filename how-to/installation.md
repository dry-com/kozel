# Kozel Setup Instructions

## Preparation Before Using Kozel (Based on Operating System)

### macOS:
1. Download Docker from this link: [Docker Documentation](https://docs.docker.com/desktop/setup/install/mac-install/).
2. Install Socat. You can install it with Homebrew using the command:
   ```bash
   brew install socat

## Linux

1. Download and install Docker from the [Docker Documentation](https://docs.docker.com/desktop/setup/install/linux/).
2. Or you can use these commands in the terminal:
   ```bash
   sudo apt update
   sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   sudo curl -L "https://github.com/docker/compose/releases/download/v2.29.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
   sudo chmod +x /usr/local/bin/docker-compose
   docker-compose --version

## Windows

1. Download and install Docker from the [Docker Documentation](https://docs.docker.com/desktop/setup/install/windows-install/).
2. During installation, ensure you check the appropriate box as shown in the image below:
![telegram-cloud-photo-size-2-5294071140131661243-y](https://github.com/user-attachments/assets/1a37bfc6-3027-4dfb-944b-aa1be863ca4a)


