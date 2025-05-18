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
- Create bckend role for contenerizing backend role
    - use community.docker.image to build image and add necessary args
    - spin off container from build image
```