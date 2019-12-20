# Installation Docker

See documentation [Docker ce Ubuntu18.04](ihttps://docs.docker.com/install/linux/docker-ce/ubuntu/)


## Unistall old Version

To install Docker Engine - Community, you need the 64-bit version of one of these Ubuntu versions:

*    	Disco 19.04
*    	Cosmic 18.10
*    	Bionic 18.04 (LTS)
*	Xenial 16.04 (LTS)

Older versions of Docker were called docker, docker.io , or docker-engine. If these are installed, uninstall them:

```
sudo apt-get remove docker docker-engine docker.io containerd runc
```


If you cannot use Docker’s repository to install Docker Engine - Community, you can download the .deb file for your release and install it manually. You need to download a new file each time you want to upgrade Docker.

## Install from a package

* Go to https://download.docker.com/linux/ubuntu/dists/, choose your Ubuntu version, browse to pool/stable/, choose amd64, armhf, arm64, ppc64el, or s390x, and download the .deb file for the Docker Engine - Community version you want to install.

* Install Docker Engine - Community, changing the path below to the path where you downloaded the Docker package.

```
sudo dpkg -i /path/to/package.deb
```

* The Docker daemon starts automatically. Verify that Docker Engine - Community is installed correctly by running the hello-world image.

```
sudo docker run hello-world
```




