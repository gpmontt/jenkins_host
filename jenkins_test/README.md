# Installation Jenkins Server

What you need is:
- Docker CE compatibel with your system
- Install Docker-compose 
- image from [official jenkinsci](https://hub.docker.com/r/jenkinsci/blueocean) `docker pull jenkinsci/blueocean`

ref [install jenkins on docker](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-18-04)

# Run service

The file `docker-compose.yaml` have the rules to create the service `jenkinsci_blueocean` on docker. 
We are using the `docker.sock` to  the process to access in the docker container.
We will created together with the service `jenkinsci_blueocean` the volumen `jenkins_home`, where all your stuff is allocated.

Then run:
```
docker-compose up -d 
```

If you write `docker ps`  

![ref](https://jpetazzo.github.io/assets/archer.jpg)
