# Dev Box using Vagrant and Librarian
Optimized for rails development with PostgreSQL and MongoDB
Can be customized as needed

## Setup
- Download and Install Virtual Box
- Download and Install Vagrant
- Download this repo into your project's root directory
- gem install librarian-chef
- vagrant plugin install vagrant-librarian-chef

## To Use
- vagrant up
- vagrant ssh
- cd vagrant
- Edit code on host machine
- execute in command line on guest machine

## Included Packages

### Vagrant
Uses Virtual Box to quickly create and use headless VMs for development

### Chef
Uses a Ruby DSL to provision machines (ie the Vagrant VM) with the appropriate software.  Uses "cookboks" which can be shared with the community to define setup instructions for diffearent applications.  See http://community.opscode.com/

### Librarian-Chef
Bundler for chef cookbooks.  Automatically downloads and updates cookbooks as defined in chef/Cheffile.

### Vagrant-Librarian-Chef
Automatically runs Librarian-Chef when creating a new box with "vagrant up", or calling "vagrant provision".