# Cloud Infrastructure and Server Automation Using AWS and Ansible - DevOps Lab Assignment 5
Student Name: Yuvraj Shembale  
PRN: 123B1D045  

Automating the installation, configuration, and deployment of an Nginx web server on an AWS EC2 instance using Ansible.

## Key Steps
1. Configure \inventory.ini\ with target EC2 host IP and private key file.
2. Verify SSH connectivity using ad-hoc ping:
   \\\ash
   ansible webservers -i inventory.ini -m ping
   \\\
3. Run the playbook to provision and deploy Nginx:
   \\\ash
   ansible-playbook -i inventory.ini site.yml
   \\\
4. Verify the web server in browser at \http://<EC2_PUBLIC_IP>\.
5. Run the playbook a second time to demonstrate **Ansible idempotency** (\changed=0\).
