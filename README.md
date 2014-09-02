-*- mode: markdown; mode: auto-fill; fill-column: 80 -*-

# Public [ULHPC](http://hpc.uni.lu) Puppet roles

[![Puppet Forge](http://img.shields.io/puppetforge/v/ULHPC/public_roles.svg)](https://forge.puppetlabs.com//ULHPC/public_roles)
[![License](http://img.shields.io/:license-apache2.0-blue.svg)](LICENSE)
![Supported Platforms](http://img.shields.io/badge/platform-debian-lightgrey.svg)

Public Puppet ULHPC roles to be used in r10k environments

      Copyright (c) 2014 S. Varrette, H. Cartiaux, V. Plugaru <hpc-sysadmins@uni.lu>
      

* [Online Project Page](https://github.com/ULHPC/puppet-public_roles)  -- [Sources](https://github.com/ULHPC/puppet-public_roles) -- [Issues](https://github.com/ULHPC/puppet-public_roles/issues)

## Synopsis

Public Puppet ULHPC roles to be used in r10k environments, typically in Vagrant
boxes -- see [vagrant-vms](https://github.com/Falkor/vagrant-vms) for instance.

The various operations of this repository are piloted from a `Rakefile` which
assumes that you have [RVM](https://rvm.io/) installed on your system.

## Dependencies

See `metadata.json`.

## Usage

You can see how this module is used in our
[Public Puppet Infrastructure repository](https://github.com/ULHPC/puppet-public_infrastructure).  

## Librarian-Puppet / R10K Setup

You can of course configure ULHPC-public_roles in your `Puppetfile` to make it 
available with [Librarian puppet](http://librarian-puppet.com/) or
[r10k](https://github.com/adrienthebo/r10k) by adding the following entry:

     mod ULHPC-public_roles, 
         :git => https://github.com/ULHPC/puppet-public_roles,
         :ref => production 


## Issues / Feature request

You can submit bug / issues / feature request using the 
[ULHPC/public_roles Tracker](https://github.com/ULHPC/puppet-public_roles/issues). 


## Developments / Contributing to the code 

If you want to contribute to the code, you shall be aware of the way this module
is organized.
These elements are detailed on [`doc/contributing.md`](doc/contributing.md)

You are more than welcome to contribute to its development by 
[sending a pull request](https://help.github.com/articles/using-pull-requests). 

## Resources

### Git 

You should become familiar (if not yet) with Git. Consider these resources: 

* [Git book](http://book.git-scm.com/index.html)
* [Github:help](http://help.github.com/mac-set-up-git/)
* [Git reference](http://gitref.org/)

### r10k, Roles and Profiles

* [r10k reference](https://github.com/adrienthebo/r10k) --
  [Puppetfiles](https://github.com/adrienthebo/r10k/blob/master/doc/puppetfile.mkd)
  and
  [dynamic environment deployment](https://github.com/adrienthebo/r10k/blob/master/doc/dynamic-environments.mkd)
  documentations
* a [Puppet Tutorial](https://github.com/rnelson0/puppet-tutorial) bootstrapping
  a similar configuration, including
  [profiles](https://github.com/rnelson0/rnelson0-profile) and
  [roles](https://github.com/rnelson0/rnelson0-role) -- see
  [Puppet for Vsphere admins](http://rnelson0.com/puppet-for-vsphere-admins/)
* __r10k tutorials__:
  * [Gary Larizza blog](http://garylarizza.com/blog/2014/02/18/puppet-workflow-part-3/),  
  * [Hunner](https://github.com/hunner/roles_and_profiles)
