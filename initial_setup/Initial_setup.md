Installed RHEL on both of my servers.

I want to setup cockpit so I can have web-based monitoring and management of my server. 
I also want to setup ansible for configuration management. 

Cockpit Notes:
- I had to register to the red hat network before installing any software packages.
  - Resources/guide : https://www.dell.com/support/kbdoc/en-us/000215142/linux-yum-update-fails-with-the-message-error-the-system-is-not-registered-with-an-entitlement-server-you-can-use-subscription-manager-to-register
- I already ended up having cockpit installed, funnily enough. enabled the process using this command : sudo systemctl enable --now cockpit.socket

Ansible Notes:
- After looking around at articles/videos on ansible / installing ansible I feel confident to install.
- PIP seems like the best way to install ansible.
- I will be install ansible on a virtual machine seperate from the lab machines.
- I need the most up to date version of python. Based on the ansible-core support matrix, the version of python that came by default, python 3.9, is already eol for ansible-core
  - https://docs.ansible.com/ansible/latest/reference_appendices/release_and_maintenance.html#support-life
- This video covered everything for the installation. Seems to be best practice and its pretty recent. :
  - https://www.youtube.com/watch?v=E274Lv1QhDg
- After installation I wanted to do a simple ping test of my host machines
  - https://www.redhat.com/en/blog/ansible-quick-start
- "ansible all -m ping -i inventory.yaml" successfully reached out to the hosts. 
