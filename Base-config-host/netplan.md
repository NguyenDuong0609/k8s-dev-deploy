path: /etc/netplan/00-install-config.yaml

content:
network:
  version: 2
  ethernets:
    ens33:
      dhcp4: false
      addresses:
        - 192.168.101.55/24
      routes:
        - to: default
          via: 192.168.101.1
      nameservers:
        addresses:
          - 8.8.8.8
          - 1.1.1.1
