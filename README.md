# DevOps Home Test

This repo is for all interviewees to attempt TheScore's take home test

## Instructions
The headings below are related to each task you must finish to complete the DevOps Take-Home Test. We will provide you with a private key so that you can SSH into the instance.

### Python
Write a simple python script that will fetch a json feed and extract the information required to create a host file that will later to be used by ansible.

### Hello World App
Create an application using any programming language you wish (python,ruby,node, etc...) that will live within a container that returns a simple `Hello World! $(HOSTNAME)`. We want this to be dynamic and show a hostname so we can see it can gather information from the container.

### Dockerfile
Write a Dockerfile that has all the dependencies and steps to build a container to host the Hello World App you created in the previous step. Make sure to write this file so that I can clone the branch and run docker build to create the container. 

### Ansible Playbook
Please feel free to make this as simple or complex as you wish but it should be called deploy.yml
Make sure the playbook does the following:
  - Install Docker
  - Get the required files on the machine to build the container using the Dockerfile
  - Make sure all your work is done in `/root/app`
  - Run the container as a daemon
  - Make sure the application is accessible from the internet
