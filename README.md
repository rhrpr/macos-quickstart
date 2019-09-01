macos-quickstart is designed to setup my MacOS workstation with both the tools I use on a regular basis.

Requirements
------------

Ansible ~> 2.7.x

Role Variables
--------------

/group_vars/all sets the packages you wish to install via homebrew or homebrew cask


Dependencies
------------

Roles;
geerlingguy.homebrew
elliotweiser.osx-command-line-tools


Usage
------------

Check the list of Packages in /group_vars/all and set to your preferences.

Check for existing brew packages using [Search Brew](http://searchbrew.com/)

Check for existing casks in [The Brew Casks Repo](https://github.com/Homebrew/homebrew-cask/tree/master/Casks)

Run as BECOME sudo to install packages via brew

`ansible-playbook playbook.yml -K`
