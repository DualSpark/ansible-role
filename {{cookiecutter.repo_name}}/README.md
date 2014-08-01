# {{ cookiecutter.repo_name }}

{{ cookiecutter.project_short_description }}

## Requirements

This solution has a vagrantfile for use in testing the Ansible Role contained within this repo. As such, the following programs are required to fully utilize the [Vagrant](http://www.vagrantup.com) test solution:

* [Vagrant](http://www.vagrantup.com/download) - tested with v1.6.3
* [Ansible](http://www.ansible.com) - tested with v1.6.6

### Ansible install via pip

The enclosed requirements.txt file includes details to install the proper version ({{ cookiecutter.ansible_version }}) of Ansible for this project. To install, use the following command within a terminal window from this directory:

```bash
pip install -r requirements.txt
```

### Vagrant info

This project is configured to use a box that is named {{ cookiecutter.vagrant_box_name }} locally - this points to the Vagrant Box located [here]({{ cookiecutter.vagrant_box_url }}). If you do not have a box by this name locally, please note that the first time you run ```vagrant up``` to test this project, you'll start the process with Vagrant downloading the box file. This can take some time depending on your connection, but on subsequent launches, initlialization of the Vagrant Box will not require a download for the image itself. 

### Helpful Vagrant Plugins

The following are plugins to Vagrant that you might find helpful. Installation of these plugins is accomplished by executing the following (after Vagrant itself is installed):

```bash 
vagrant plugin install __plugin-name__
```

* [vagrant-pristine](https://github.com/fgrehm/vagrant-pristine) - makes destroying and re-creating an environment a little easier by using one command (with a switch to force): ```vagrant pristine -f```
* [landrush](https://github.com/phinze/landrush) - dns manager using dnsmasq or host files to allow for friendlier naming and cross-system access both between multiple guests as well as from the host to the guest. 

#####created with [ansible-role](https://github.com/DualSpark/ansible-role) cookiecutter template