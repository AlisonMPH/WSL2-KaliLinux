# WSL2-KaliLinux
#### Instalando o Kali no Windows

ð¦ð¦ð¦COMMANDS:ð¦ð¦ð¦

1. INSTALL WSL 2

RUN POWERSHELL as administrator

âï¸ Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

RESTART

âï¸ dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

âï¸ dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

RESTART

Download Linux Kernel: https://aka.ms/wsl2kernel

SET DEFAULT TO WSL 2
âï¸ wsl --set-default-version 2

CHECK VERSION 
âï¸ wsl --list --verbose

2. INSTALL GUI

âï¸ sudo apt update && sudo apt upgrade -y

âï¸ sudo apt install kali-desktop-xfce -y

XRDP

âï¸ sudo apt install xrdp -y

âï¸ sudo service xrdp start

Video: https://www.youtube.com/watch?v=AfVH54edAHU
