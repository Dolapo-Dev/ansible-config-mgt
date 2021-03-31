# ansible-config-mgt. 
##To resolve the following error below:
{"msg": "Using a SSH password instead of a key is not possible because Host Key checking is enabled and sshpass does not support this. Please add this host's fingerprint to your known_hosts file to manage this host."}  
### Do the following
Create a file ansible/ansible.cfg in your project directory (i.e. ansible.cfg in the provisioning_path on the target) with the following contents:
[defaults]
host_key_checking = false
