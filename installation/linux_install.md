# Kozel Setup Instructions Linux

## 1. Install Docker
1. Download and install Docker from the [Docker Documentation](https://docs.docker.com/desktop/setup/install/linux/).
2. Or you can use these commands in the terminal:
   ```bash
   sudo apt update
   sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   sudo curl -L "https://github.com/docker/compose/releases/download/v2.29.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
   sudo chmod +x /usr/local/bin/docker-compose
   docker-compose --version```

If you will have problem with docker like `unable to configure the Docker daemon with file /etc/docker/daemon.json: the following directives are specified both as a flag and in the configuration file: hosts: (from flag: [fd://], from file:`
try to run
```
sudo cp /lib/systemd/system/docker.service /etc/systemd/system/
sudo sed -i 's/\ -H\ fd:\/\///g' /etc/systemd/system/docker.service
sudo systemctl daemon-reload
sudo systemctl restart docker
```

## 2. Install latest version of Kozel

https://github.com/user-attachments/assets/fceb2b0a-1742-4e3f-bba6-868f149423cb

1. Visit the [release page](https://github.com/dry-com/kozel/releases) and choose the most recent Kozel release.
2. Please choose the appropriate version to download based on your operating system.
3. After downloading the application file, you will need to remove any restrictions by using the following command:
   ```bash
   xattr -d com.apple.quarantine /path/to/file
   
4. After successfully installing the application, install the necessary tools for its proper operation.

<img width="1105" alt="download_tools" src="https://github.com/user-attachments/assets/44d83618-334b-447a-a044-d0f7ff8b2fbf" />
<img width="1105" alt="download_tools_approve" src="https://github.com/user-attachments/assets/ad925b82-834e-49d2-a47d-5946808aedf3" />

If you have any questions or suggestions, please use the links below:

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/hidden_coding)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HiddenCodeDevs/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/hidden_coding)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@flaming_chameleon)
