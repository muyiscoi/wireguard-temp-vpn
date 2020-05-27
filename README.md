# wireguard-temp-vpn
Create a temporary droplet configured as a wireguard VPN server and configure local machine to use it

## Requirements

- Ubuntu 20.04 or newer
- dopy (from pip)

## Usage

To create droplet and configure VPN on both server and client,

```
ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook create.yml
```

To disconnect client and delete VPN server droplet

```
ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook cleanup.yml
```