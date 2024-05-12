# dotfiles_fedora
Personal setup for my Fedora installation. Including instructions and dotfiles

## Installation
- Do basic installation of Fedora with `Secure Boot` enabled
- Install nvidia drivers [Nvidia isntall link](https://rpmfusion.org/Howto/NVIDIA)
- Setup keys for secure boot for nvidia
    - [Secure boot setup link](https://rpmfusion.org/Howto/Secure%20Boot)
    - Run this to generate keys `sudo kmodgenca -a`
    - Run this to enroll the keys `sudo mokutil --import /etc/pki/akmods/certs/public_key.der`
    - Reboot
    - On the next boot MOK Management is launched and you have to choose "Enroll MOK" 
