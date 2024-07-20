# Wireguard for Ansible
## Install ansible
Open a terminal on your Linux machine.
Install Ansible using your package manager:
For Ubuntu/Debian: 
``` 
sudo apt-get install ansible 
```
For Red Hat/CentOS/Fedora: 
``` 
sudo yum install ansible 
```
For openSUSE: ``` 
sudo zypper install ansible 
```
Verify the installation by running:
``` 
ansible --version 
```
This should display the version of Ansible installed on your machine.

## Clone the repo into your machine
``` 
git clone https://github.com/intaky-dev/wireguard-ansible.git 
```
## Run the ansible playbook with
``` 
ansible-playbook wireguard-playbook.yml 
```

## Replace your variables in the wireguard-playbook.yml file 
``` 
vars: 
  users: 
    - user: "user1"
      ip: "10.0.0.2/32"
    - user: "user2"
      ip: "10.0.0.3/32"
    - user: "user3"
      ip: "10.0.0.4/32"  
  wireguard_interface: wg0
  tables_interface: eth0
  server_ip: "10.0.0.1/24"
  client_ip: "10.0.0.2/32"
  listen_port: 51820
  dns_servers: "10.42.0.1 , 8.8.8.8"
  local_ip: "10.42.0.0/24"
  end_point: "INSERT YOUR ENDPOINT HERE" 
```  