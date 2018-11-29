# ansible-rhel8
Playbooks that automate some cool stuff in RHEL 8

composer.yaml  
-------------------
Composer website : https://github.com/weldr/lorax

This playbook will install and configure everything Composer needs to work. 

Requirements : 
  1. copy the BaseOS and the Appstream directory from the RHEL 8 iso in a directory  
  2. ansible-galaxy install linux-system-roles.firewall
  3. RHEL 8 Beta requires some tricks to work with Ansible : 
  3.1 yum -y module install python36
  3.2 Add this line in your inventory file on each host : ansible_python_interpreter=/usr/libexec/platform-python 
  more information can be found here : https://www.ansible.com/blog/integrating-ansible-and-red-hat-enterprise-linux-8-beta 
       
