# tasks

## setup

### requirements
 - vagrant
 - virtualbox 

### clone repository

`git clone git@github.com:gon64/vagrant-tasks.git`

### set up vagrant vms

run the command `vagrant up` from a terminal

## vagrant structure

### machines
There's two machines running:
 - dev
 - sta

each one of them will run one of the diferent enviroments (developement, staging)

### networking
 - dev is port forwarding 80 (guest) => 8181 (host)
 - sta is port forwarding 80 (guest) => 8282 (host)

so you can easyly access to the running website just accessing to http://localhost:8181 or http://localhost:8282

## TODO