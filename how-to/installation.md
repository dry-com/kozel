# Kozel Setup Instructions

## Preparation Before Using Kozel (Based on Operating System)

### macOS:



https://github.com/user-attachments/assets/fceb2b0a-1742-4e3f-bba6-868f149423cb




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
   docker-compose --version```

If you will have problem with docker like `unable to configure the Docker daemon with file /etc/docker/daemon.json: the following directives are specified both as a flag and in the configuration file: hosts: (from flag: [fd://], from file:`
try to run
```
sudo cp /lib/systemd/system/docker.service /etc/systemd/system/
sudo sed -i 's/\ -H\ fd:\/\///g' /etc/systemd/system/docker.service
sudo systemctl daemon-reload
sudo systemctl restart docker
```






## Windows

1. Download and install Docker from the [Docker Documentation](https://docs.docker.com/desktop/setup/install/windows-install/).
2. During installation, ensure you check the appropriate box as shown in the image below:
![telegram-cloud-photo-size-2-5294071140131661243-y](https://github.com/user-attachments/assets/1a37bfc6-3027-4dfb-944b-aa1be863ca4a)

# Инструкции по настройке Kozel

## Подготовка перед использованием Kozel (в зависимости от операционной системы)

### macOS:
1. Скачайте Docker по ссылке - [Docker Documentation](https://docs.docker.com/desktop/setup/install/mac-install/).
2. Скачайте Socat. Вы можете скачать его с помощью Homebrew через команду:
   ```bash
   brew install socat

## Linux

1. Скачайте Docker по ссылке - [Docker Documentation](https://docs.docker.com/desktop/setup/install/linux/).
2. Или запустите эти команды в консоли:
   ```bash
   sudo apt update
   sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   sudo curl -L "https://github.com/docker/compose/releases/download/v2.29.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
   sudo chmod +x /usr/local/bin/docker-compose
   docker-compose --version

## Windows

1. Скачайте Docker по ссылке - [Docker Documentation](https://docs.docker.com/desktop/setup/install/windows-install/).
2. Поставьте галочку, как на фото:
![telegram-cloud-photo-size-2-5294071140131661243-y](https://github.com/user-attachments/assets/1a37bfc6-3027-4dfb-944b-aa1be863ca4a)


