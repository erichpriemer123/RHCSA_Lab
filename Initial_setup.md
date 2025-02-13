Installed RHEL on both of my servers.

I want to setup cockpit so I can have web-based monitoring and management of my server.  

Notes:
- I had to register to the red hat network before installing any software packages.
  - Resources/guide : https://www.dell.com/support/kbdoc/en-us/000215142/linux-yum-update-fails-with-the-message-error-the-system-is-not-registered-with-an-entitlement-server-you-can-use-subscription-manager-to-register
- I already ended up having cockpit installed, funnily enough. enabled the process using this command : sudo systemctl enable --now cockpit.socket
