# Project walkthrough
1. set up vm machine
```
- Generate Varant file with vagrant init geerlingguy/ubuntu2004
- Add  instruction to allow playbook.yml to be run by ansible.
- Create ansible.cfg to set up vm access variables
    - inventory
    - remote user
    - private key
```
2. create roles folder for the different roles i.e backend, fronend, db.
```
- Create backend role for contenerizing backend role
    - use community.docker.image to build image and add necessary args
    - spin off container from build image
    - create envinment variables for this role
    - add backend container to the same network as the Db to allow for communication

- Create frontend role for contenerizing frontend 
    - use community.docker.image to build image and add necessary args
    - spin off container from build image

- Create mongo role for contenerizing mongo db
    - create the network that the container will use
    - use community.docker.image to build image and add necessary args
    - spin off container from build image
```
3. playbook yaml for ansible
```
    - create pre-task to check if docker is installed
    - if docker is not available install docker
    - clone project from github into virtual machine
    - run roles in virtual machine to create the different containers
```