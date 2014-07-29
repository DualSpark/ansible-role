# ansible-role 

Cookiecutter template for Ansible roles. See https://github.com/audreyr/cookiecutter.

* Free software: [ISC license](http://en.wikipedia.org/wiki/ISC_license)
* Ansible Roles get created with [Travis-CI](http://travis-ci.org) testing 
* Template stubs out all commonly used folders with simple .dir_info descriptions 

## What's included in the Ansible role that's stubbed out?

A few things:   

* basic folder structure with brief description of folder contents in .dir_info files
* Vagrantfile and proper configuration to allow for siloed testing of the Role
* Python and Vagrant-targeted .gitignore file

## Usage

To use this, you must first install the cookiecutter puthon package:

```bash
pip install --upgrade cookiecutter
```

Generate an Ansible role project:

```bash
cookiecutter https://github.com/DualSpark/ansible-role.git
```

or

```bash
cookiecutter git@github.com:DualSpark/ansible-role.git
```

**Then:** 

* Initialize a repo, commit all the bits and push!
* Add the repo to your Travis CI account
* Write your awesome Ansible role
* Register your role with [Ansible Galaxy](https://galaxy.ansible.com/)

## Parameter Definitions

| Parameter | Default | Description | 
|---|---|---| 
| full_name  | Patrick McClory  | Author's name.  |
| email  | patrick@dualspark.com  | Author's email.  |
| project_name  | Ansible Role Boilerplate  | Friendly name for the project.  |
| repo_name  | ansible-boilerplate  | Name of the repository to hold the new role being created.  |
| role_name  | boilerplate  | Name of the role to be created.  | 
| project_short_description  | Ansible role boilerplate contains all the boilerplate to create a fully-baked Ansible role.  | 
| ansible_version  | 1.6.6  | Version of Ansible to use when testing the role being developed.  | 
| vagrant_box_url  | https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box  | URL that Vagrant will use to retrieve the base Vagrant image from  |
| vagrant_box_name  | trusty64  |  Vagrant Box name to use as an alias for the box downloaded from vagrant_box_url  |
| role_hosts  | all  | Ansible configuration that indicates which hosts should have the role deployed  |
| role_use_sudo  | true  | Indicates that Ansible should use sudo when calling commands in the role definition yml file  |
| release_date  | 2014-07-07  | Date that repo is to be/was released  | 
| year  | 2014  | Year that repo is to be/was released  |
| version  | 0.1.0  | Initial version of the role being created  | 

