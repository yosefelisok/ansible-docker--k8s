# jenkins-docker--k8s


Deployment of python program hello-boris.py via Jenkins pipeline (jenkinsfile is named jenkinsfinalversion ) 

GIT => Jenkins Server => DockerHUb image => Pod in Kubernetes Cluster in EC2 AWS

Stages
  1. Cloning Git https://github.com/yosefelisok/ansible-docker--k8s with the application hello-boris
  2. Building image for Docker using Dockerfile and requirements.txt file
  3. Deploy Image in public DockerHub repository https://hub.docker.com/repository/docker/yosefeli/leumi-pr
  4. Remove Unused docker image
  5. Deploy to DevServer in AWS EC2 server with installed kubernetes cluster using deployment files service.yml and pods.yml
