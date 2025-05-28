# Windows

Script:
- Set-ItemProperty -Path "HKLM:\SOFTWARE\Microsoft\Cryptography" -Name "MachineGuid" -Value ([guid]::NewGuid()).Guid

# Linux

Script:
- sudo systemctl stop systemd-machine-id-commit.service

- sudo rm /etc/machine-id

- sudo rm /var/lib/dbus/machine-id

- sudo systemd-machine-id-setup

- cat /etc/machine-id

- sudo reboot
