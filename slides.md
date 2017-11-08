% Ansible 2.4, 2.5, AWX
% Will Thames
% 09 November 2017

# Or, Notes from AnsibleFest SF

* Thanks to Ansible
* Thanks to XVT

# Ansible 2.4

* Released during AnsibleFest (early September)
* Python 3 core support
* YAML configuration
* Pluggable inventory (see resources later)
* Per-role vault passwords
* Better Azure support
* Massive Networking updates
* Powershell DSC support

# Red Hat Ansible Engine

* Red Hat now provide support for Ansible's core engine
  and 100 or so core modules.

# Ansible Tower 3.2

* Prioritize and group Tower nodes
* Isolate Tower nodes (no outbound traffic)
* Fact cache, smart inventories
* SCM controlled inventories (thanks!)

# AWX

* Upstream open source project for Ansible Tower
* Ansible Tower releases will be cut from AWX
* FAQ: What does it stand for?

# Some other asides

* Working groups are really taking off
    - Windows (talk to Jordan)
    - AWS (talk to me)
    - VMWare
    - Networks
* And many more - [https://github.com/ansible/community](https://github.com/ansible/community)

# Ansible 2.5

Still no published roadmap, not much of note in the changelog.
From an AWS point of view:

* AWS dynamic inventory will be converted to plugins
* More support for AWS Serverless Application Model
* More boto3 modules

# Notes from Ansible 2.4 release

I introduced a lot of AWS bugs into Ansible 2.4, and then
fixed a lot of those bugs for 2.4.1.

To avoid this, all improvements to AWS modules marked as
`stableinterface` require tests. This might slow down boto3
migration, but we should be able to spend less time fixing
bugs and more time migrating!

10% of Ansible modules are AWS! (Networks modules comprise
a higher proportion though)

# Ansible 2.4 blog posts

* [Testing AWS Modules](http://willthames.github.io/2017/07/17/so-you-want-to-test-aws-modules-for-ansible.html)
* [Generating Inventory](http://willthames.github.io/2017/11/01/generating-inventory.html)

# AnsibleFest talk highlight

* [Infrastructure Testing with Molecule](https://www.ansible.com/infastructure-testing-with-molecule)
* [Ansible and Serverless](https://www.ansible.com/ansible-and-serverless-technologies)

