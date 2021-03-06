# vagrant-berkshelf

[![Gem Version](https://badge.fury.io/rb/vagrant-berkshelf.png)](http://badge.fury.io/rb/vagrant-berkshelf)
[![Build Status](https://travis-ci.org/berkshelf/vagrant-berkshelf.png?branch=master)](https://travis-ci.org/berkshelf/vagrant-berkshelf)
[![Dependency Status](https://gemnasium.com/berkshelf/vagrant-berkshelf.png)](https://gemnasium.com/berkshelf/vagrant-berkshelf)

A Vagrant plugin to add Berkshelf integration to the Chef provisioners

## Installation

Install Vagrant '>= 1.5.2' from the [Vagrant downloads page](http://www.vagrantup.com/downloads.html)

Install the Vagrant Berkshelf plugin

    $ vagrant plugin install vagrant-berkshelf --plugin-version '>= 2.0.1'

## Usage

Once the Vagrant Berkshelf plugin is installed it can be enabled in your Vagrantfile

    Vagrant.configure("2") do |config|
      ...
      config.berkshelf.enabled = true
      ...
    end

The plugin will look in your current working directory for your `Berksfile` by default. Just ensure that your Berksfile exists and when you run `vagrant up`, `vagrant provision`, or `vagrant destroy` the Berkshelf integration will automatically kick in!

## Getting Help

* If you have an issue: report it on the [issue tracker](https://github.com/berkshelf/berkshelf/issues)
* If you have a question: visit the #chef or #berkshelf channel on irc.freenode.net

# Authors

- Jamie Winsor (<jamie@vialstudios.com>)
- Michael Ivey (<michael.ivey@riotgames.com>)

Thank you to all of our [Contributors](https://github.com/berkshelf/vagrant-berkshelf/graphs/contributors), testers, and users.

If you'd like to contribute, please see our [contribution guidelines](https://github.com/berkshelf/vagrant-berkshelf/blob/master/CONTRIBUTING.md) first.
