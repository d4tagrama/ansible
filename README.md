
- **File list**
	- [CentOS-PHP](ansible/centos-php.yml)


## Quick Start

Add IP address of all hosts to `/etc/ansible/hosts`  and  execute the playbook you need:


- **Install php 7.X**

	Execute the command:

		ansible-playbook -u <user> <playbook.yml>  --extra-var "major_version=<major_version>"
	
	 - `<user>`: Specify the user to execute the playbook. The user need `sudo` privileges to run
	 - `<playbook.yml>`: Playbook file
	 - `<major_version>`: Major version variable if you are using multiple vars use `--extra-vars '{"major_version":7,"enablerepo":remi-php72}'`


## Examples:

- Install php 7.2:

		ansible-playbook -u usradm centos-php.yml  --extra-vars '{"major_version":7,"enablerepo":remi-php72}'
		ansible-playbook -u usradm centos-php.yml  --extra-vars '{"major_version":7,"enablerepo":remi-php73}'


