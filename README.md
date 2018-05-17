# Ansible-SSHKeys
An Ansible-playbook for deploying or managing SSH keys. 

A very simple ansible playbook to deploy user specified SSH keys straight out of the documentation.
[Refrence Documentation Here.](http://docs.ansible.com/ansible/latest/authorized_key_module.html)

# To Use:
Just change the taged values in the .yml file and off you go. 

I intend to write a wrapper for this so it can be executed from command line with the remote user, deploy user, and key location as options for simplicity and quick adding, but hey, have to have time and modivation for that xp.

# Quick ansible how to:
ansible-playbook <options> ./Ansible-DeploySSHKeys.yml
* -i <host>, == Specify an invintory file or a host followed by a comma
* -e 'host_key_checking=False' == If you have multiple systems that you havent yet logged into
* -k == user login password prompt
* -K == sudo password in case you want to deploy as root and have a sudo password
* --private-key <keyfile> == If you intend to log into a system with a keyfile (eg. your rotating keys)
