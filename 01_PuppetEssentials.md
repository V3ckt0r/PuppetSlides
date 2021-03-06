# Puppet Essentials - Overview

### Introduction to Puppet

### Configuration management tools

### Puppet Ecosystem and related software


# What is Puppet

  A **Configuration Management** Tool

  A framework for **Systems Automation**

  A Declarative Domain Specific Language (**DSL**)

  An **OpenSource software** in written Ruby

  Works on Linux, Unix (Solaris, AIX, *BSD), MacOS, Windows ([Supported Platforms](http://docs.puppetlabs.com/guides/platforms.html))

  Developed by **[Puppet Labs](http://puppetlabs.com)**

  Used by [http://puppetlabs.com/customers/companies/](http://puppetlabs.com/customers/companies/) ...

  ... and **many** others


# Configuration Management advantages

  **Infrastructure as Code**: Track, Test, Deploy, Reproduce, Scale

  Code commits log shows the **history of change** on the infrastructure

  **Reproducible setups**: Do once, repeat forever

  **Scale** quickly: Done for one, use on many

  **Coherent** and consistent server setups

  **Aligned Environments** for devel, test, qa, prod nodes

  Alternatives to Puppet: [Chef](http://www.opscode.com/chef/), [CFEngine](http://cfengine.com/), [Salt](http://saltstack.com/), [Ansible](http://www.ansibleworks.com/)

# References and Ecosystem

  [Puppet Labs](http://puppetlabs.com) - The Company behind Puppet

  [Puppet](http://puppetlabs.com/puppet/puppet-open-source/) - The OpenSource version

  [Puppet Enterprise](http://puppetlabs.com/puppet/puppet-enterprise/) - The commercial version

  [The Community](http://puppetlabs.com/community/overview/) - Active and vibrant

  [Puppet Documentation](http://docs.puppetlabs.com/) - Main and Official reference

  Puppet Modules on: [Module Forge](http://forge.puppetlabs.com) and [GitHub](https://github.com/search?q=puppet)

# Software related to Puppet:

  [Facter](http://docs.puppetlabs.com/facter/) - Complementary tool to retrieve system's data

  [MCollective](http://docs.puppetlabs.com/mcollective/) - Infrastructure Orchestration framework

  [Hiera](http://docs.puppetlabs.com/hiera/1/) - Key-value lookup tool where Puppet data can be placed

  [PuppetDB](http://docs.puppetlabs.com/puppetdb/1/) - Stores all the data generated by Puppet

  [Puppet DashBoard](http://docs.puppetlabs.com/dashboard/) - A Puppet *Web frontend* and External Node Classifier (ENC)

  [The Foreman](http://theforeman.org/) - A well-known third party provisioning tool and Puppet ENC

  [Geppetto](http://cloudsmith.github.com/geppetto) - A Puppet IDE based on Eclipse


# Installation

  Debian, Ubuntu
  Available by default

    apt-get install puppet       # On clients (nodes)
    apt-get install puppetmaster # On server (master)

  RedHat, Centos, Fedora
  Add EPEL repository or RHN Extra channel

    yum install puppet        # On clients (nodes)
    yum install puppet-server # On server (master)

  Use [PuppetLabs repositories](http://docs.puppetlabs.com/guides/puppetlabs_package_repositories.html) for latest updates

  [Installation Instructions](http://docs.puppetlabs.com/guides/installation.html) for different OS

# Puppet Versions

From version 2 Puppet follows [Semantic Versioning](http://semver.org/) standards to manage versioning, with a pattern like: MAJOR.MINOR.PATCH

This implies that MAYOR versions might not be backwards compatible, MINOR versions may introduce new features keeping compatibility and PATCHes are for backwards compatible bug fixes.

This is the history of the main Puppet versions and some relevant changes
Check also [Puppet Language History](http://docs.puppetlabs.com/guides/language_history.html) for a more complete review:

  0.9.x  - First public beta

  0.10.x - 0.21.x - Various "early" versions

  0.22.x - 0.25.x - Improvements and OS wider support

  2.6.x  - Many changes. Parametrized classes

  2.7.x  - Windows support

  3.0.x  - Many changes. Disabled dynamic variables scope. Data bindings

  3.2.x  - Future parser (experimental, will be default in Puppet 4)

  4.x.x  - Release in early 2015. New parser, new type system and lot of changes, some backwards incompatibilities
