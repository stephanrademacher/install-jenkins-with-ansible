Simple playbook to install jenkins on a hosts

it assumes 
- you have a linux vm 
- you have a ssh trust between ansible host and linux vm


steps: 

- installs git 
- installs geerlingguy.jenkins via ansible-galaxy
- configures plugins and installs them ( see plugins.txt )
- open port 8080 on firewall and reloads it
- restart jenkins
