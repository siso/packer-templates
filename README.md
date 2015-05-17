# siso's packer-templates

[![Build Status](https://travis-ci.org/siso/packer-templates.png)](https://travis-ci.org/siso/packer-templates)

version: 0.0.0

## Synopsis

Packer templates to build Debian images for Vagrant and VirtualBox.

## Prerequisites
You will need the following software on your local host:
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- [Vagrant](http://www.vagrantup.com/downloads.html)

## Quickstart

```shell
# build debian jessie image for virtualbox
packer build debian-8.0.0-amd64-virtualbox.json

# add vagrant box
vagrant box add siso-debian-8.0.0-amd64-jessie virtualbox/siso-debian-8.0.0-amd64-jessie.box

# create vagrant project
vagrant init

# edit Vagrantfile, and set 'config.vm.box = "siso-debian-8.0.0-amd64-jessie"'

# start and ssh into box
vagrant up
vagrant ssh

# destroy and remove box
vagrant destroy
vagrant box remove siso-debian-8.0.0-amd64-jessie
```

## Links

- [Packer](https://www.packer.io/)

## Contribute

- Fork the repository on Github
- Create a named feature branch (like add_component_x)
- Write your change
- Write tests for your change (if applicable)
- Run the tests, ensuring they all pass
- Submit a Pull Request using Github

## Authors

- Author:: Simone Soldateschi (simone.soldatechi@gmail.com)

## License

Copyright (C) 2015 Simone Soldateschi

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see [http://www.gnu.org/licenses/](http://www.gnu.org/licenses/).
