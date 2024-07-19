# wireguard-ansible
## install ansible
Open a terminal on your Linux machine.
Install Ansible using your package manager:
For Ubuntu/Debian: sudo apt-get install ansible
For Red Hat/CentOS/Fedora: sudo yum install ansible
For openSUSE: sudo zypper install ansible
Verify the installation by running:
ansible --version
This should display the version of Ansible installed on your machine.


replace your variables in the wireguard-playbook.yml file 
vars:
    wireguard_interface: wg0 ##default
    tables_interface: eth0 ##default
    server_ip: "10.0.0.1/24" ##
    client_ip: "10.0.0.2/32" ##
    listen_port: 51820 ##default port
    dns_servers: "10.42.0.1 , 8.8.8.8"
    local_ip: "10.42.0.0/24"
    end_point: "INSERT YOUR ENDPOINT HERE"