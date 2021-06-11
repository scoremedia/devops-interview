# Challenge Environment

Connect to the following server:

## Server Details
```
Command: ssh ubuntu@XXXXXXXXXX
Password: XXXXXXXXXX
```

# Challenge 1 - New App
You are required to deploy a web application has built on Kubernetes.

The task is the part of that process and requires to complete a file stub "/home/ubuntu/931544-kubernetes-service-clusterip/definition.yml" with one or more steps that do the following:

* Creates a new namespace "hacker-company".
* Deploys a new "nginx" image (from Dockerhub) as "nginx" container on the "stable" tag as "frontend" pod, in the "hacker-company" namespace.
* Creates a new "role" label with the value "frontend" at the "frontend" pod.
* Creates a new "frontend" service ("ClusterIP" type), forwards "80" port of "nginx" container in "frontend" pod to the port "8080".
 

## Note

The completed solution will be evaluated in a new, clean environment. Be sure everything is in the "/home/ubuntu/931544-kubernetes-service-clusterip" folder.


# Challenge 2 - Debug Exercise
A developer deployed an elixir application to `score` namespace. They're having an issue getting the service work properlly.

Can you help?

## Details

* Application: Elixir
* Workdir: /app
* Application Pod: score-demo
* Application Config Path: `/app/config/dev.exs`

```
host: postgres
username: postgres
password: postgres
database: score_dev
```


# Challenge 3 - Python Challenge

Create a python script that can be executed from the command line to list all files and folder recursively. 

```
$ python3 list.py /home/ubuntu
```
