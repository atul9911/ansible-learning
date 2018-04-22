This module includes to setup a configuration file for ansible.
Please use following steps to create configure file for ansible.

1)Installation of Ansible:-
Prerequisite:-
1) Linux machine
2) Python >= 2.7.12

Installation of ansible on linux box:-
1) Add latest ansible repository by following command:-
	sudo apt-get install software-properties-common && sudo apt-add-repository ppa:ansible/ansible
2) Update Linux Repository
	 sudo apt-get update
3) Install the latest version of ansible
	sudo apt-get install ansible
4) Check the version of ansible installed in your machine
	ansible --version

After running 4th step you will find following output

ansible 2.5.1
  config file = /etc/ansible/ansible.cfg
  configured module search path = [u'/home/atulagrawal/.ansible/plugins/modules', u'/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/lib/python2.7/dist-packages/ansible
  executable location = /usr/bin/ansible
  python version = 2.7.12 (default, Dec  4 2017, 14:50:18) [GCC 5.4.0 20160609]


HandsOn:-
Create an ansible configuration file which will setup default ansible command timeout to 120 sec

Ansible Configuration file:-
By default when we install ansible,it will create a configuration file which we can find in /etc/ansible loccation(for ubuntu machine).

1) Run this command to make sure if ansible.cfg file is there
	cat /etc/ansible/ansible.cfg
2) Edit this file by using following command:-
	vim /etc/ansible/ansible.cfg
3) Find this line in configuration file
	# SSH timeout
	#timeout = 10
4) Uncomment the timeout =10 line and replace the value by 120.

Save and exit the file.
Now you have your ansible ssh timeout for 120sec.





