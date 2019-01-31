# DevOps Home Test

This repo is intended as a first step into theScore DevOps interview.

## Instructions
The headings below are related to each task you must finish to complete the DevOps Take-Home Test. We will provide you with a private key so that you can SSH into the instance using the `ubuntu` user.

### Python
Write a python3 script that will query an endpoint for a json object. Extract the information required to create an inventory to be used by Ansible in the subsequent tasks.

### Hello World App
Create an application using any programming language you wish (python, ruby, node, etc...) that will live within a container that returns a simple `Hello World! $(HOSTNAME)`. The output should be dynamic, and change with the hostname of the machine.

### Dockerfile
Write a Dockerfile to build a container for the app created in the previous step with all the necessary dependencies. Make sure to write this file so that anyone can `docker build` and it works.

### Minikube
Create YAML files to deploy pods and service to K8 (minikube in this case). 

### Ansible Playbook
Please feel free to make this as simple or complex as you wish but it should be called `deploy.yml`.
Make sure the playbook does the following:
  - Install Minikube, kubectl and docker (docker-ce=18.06.1~ce~3-0~ubuntu)
  - Get the required files on the machine to build the container using the Dockerfile
  - Make sure all your work is done in `/root/app`
  - Create deployment and service on minikube
  - Make sure the application is accessible from the internet on port 80

### Getting your work to us
Please send us your archived work to devops-interview[at]thescore[dot]com. It should contain instructions on how to run each individual step, as well as the URL for the hello world application.

In the interest of evaluating each candidate on their individual skillset, we request that you don't make your work publicly available. 
