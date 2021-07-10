# Dev Environment 

# Introduction

## Virtual Machine 
A **Virtual Machine (VM)** is a compute resource that uses software instead of a physical computer to run programs 
and deploy apps.Each virtual machine runs its own operating system and functions separately from the other VMs, 
even when they are all running on the same host. This means that, for example, a virtual MacOS virtual machine can run
on a physical PC. 

VMs allow a business to run an operating system that behaves like a completely separate computer in an app window on
a desktop. VMs may be deployed to accommodate different levels of processing power needs, to run software that requires
a different operating system, or to test applications in a safe, sandboxed environment. 

## Vagrant and VirtualBox
**Vagrant** is a tool for building and managing virtual machine environments in a single workflow. u a disposable
environment and consistent workflow for developing and testing infrastructure management scripts. 

**VirtualBox** is a GUI and command line tool that makes it possible to deploy servers, desktops, and embedded 
operating systems as VMs. A single VirtualBox host can deploy as many guest VMs as the host hardware can handle.



## Installation and Setup for Vagrant, VirtualBox and Ruby 
# Ruby Installation 
[Mac Ruby installation link](https://www.ruby-lang.org/en/downloads/)

- Ensure to download x64 for your OS
- Check the version on your terminal:
`ruby --version`
  
## Vagrant Installation and Setup 
[Link to vagrant download](https://www.vagrantup.com/)
 - Check version on your terminal:
`vagrant --version`
   
## VirtualBox Installation and Setup
[VirtualBox Link](https://www.virtualbox.org/wiki/Downloads)

## Testing Vagrant Installation 

- **Step 1:** From the terminal make a directory for your vagrantfile `mkdir file-name`
- **Step 2:** Put the default config file into your project directory, for the vagrant virtual machine image, known as
  a **box**, to be pulled from the public box catalog using the command:
  
  `$ vagrant init ubuntu/xenial64`

    The default config file is named Vagrantfile by convention
- **Step 4**: Now run the command `vagrant up` to bring up the virtual machine.
  Since we dont have the box for the VM available locally, vagrant will pull it form its public catalog.
  Once the box has been downloaded vagrant will configure ports to allow you to ssh into it.
- **Step 5:** With the VM running we can now ssh into the Vm by running the command:
`vagrant ssh`
  
- **Step 6:** Run the command `uname -a` to see the UNIX name, Ubuntu Linux machine.

To exit the ssh session, enter the command `exit`

To shut down the virtual machine, run the command `vagrant halt`