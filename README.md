
Ansible-Playbook und Rolle **base** für Ubuntu-Server (z. B. KVM/Cloud-Init).  
Die Rolle installiert Updates, Basis-Pakete, setzt Zeitzone, härtet SSH, aktiviert UFW und richtet automatische Updates ein.

## Voraussetzungen

- Ubuntu-Server (getestet mit 24.04 Cloud-Image)
- Zugriff via SSH mit Public-Key
- Steuerhost mit Ansible

## Nutzung

Inventar (`inventory.ini`):
```ini
[ubuntu]
vm1 ansible_host=192.168.122.171 ansible_user=holle030 ansible_ssh_private_key_file=~/.ssh/id_ed25519
