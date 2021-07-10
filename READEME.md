# Dev Environment 

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