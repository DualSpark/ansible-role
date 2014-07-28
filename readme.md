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
