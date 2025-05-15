# Windows-Reset-Machine-ID

Script:
- Set-ItemProperty -Path "HKLM:\SOFTWARE\Microsoft\Cryptography" -Name "MachineGuid" -Value ([guid]::NewGuid()).Guid
