# Overview

asdf version manager plugin for HashiCorp Vagrant

- Find asdf here    https://github.com/asdf-vm/asdf
- Find vagrant here https://www.vagrantup.com/


# Supported OS's

Currently only Linux is supported.

Mac OS is not supported due to HashiCorp distributing Vagrant as a DMG
file for Mac.


# Requirements

- curl
- md5sum
- unzip
- bash
- sed
- awk

# Vagrant Requirements

- libarchive-tools

# Install

    asdf plugin-add vagrant git@github.com:ben0x4a/asdf-vagrant.git
    asdf list-all vagrant
    
    LATEST=$(asdf list-all vagrant | tail -1)
    asdf install vagrant ${LATEST}
    asdf global vagrant ${LATEST}
    vagrant --version

