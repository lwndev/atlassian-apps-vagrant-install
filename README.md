# atlassian-apps-vagrant-install

A project that uses Vagrant and Puppet to create and boot a VirtualBox VM with the following apps

* Stash
* JIRA
* Confluence
* Bamboo

## Notes

* This is intended as a proof of concept and is not intended to be a full provisioning solution for any of the installed applications. You will need to manually supply your own licenses and use the "Evaluation Installation" option as the Puppet manifest does not install or configure a database.
* Credit where credit is due: This project is very based off-of Nicola Paolucci's Stash provisioning example https://bitbucket.org/durdn/stash-vagrant-install.git. Check out https://blogs.atlassian.com/2013/03/instant-java-provisioning-with-vagrant-and-puppet-stash-one-click-install/ for more details

## Dependencies

1. [Vagrant](http://downloads.vagrantup.com/)
2. [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## Usage

	$ git clone https://github.com/lwndev/atlassian-apps-vagrant-install.git && cd atlassian-apps-vagrant-install
	$ vagrant up

Once the boot and provisioning is complete, you can access the applications at the following locations:
* Bamboo: http://192.168.33.12:8085
* Confluence: http://192.168.33.12:8090
* JIRA: http://192.168.33.12:8080
* Stash: http://192.168.33.12:7990
