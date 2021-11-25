# **Learning Docker**
## Overview
Thank you for your interest in looking into my Github. I created this repo to showcase capabilities in working with Docker.

We are going to focus on initializing the Docker CE (Community Edition) environment in centos in simple easy steps:
1. Run `sudo yum install -y yum-utils device-mapper-persistent-data lvm2` to install docker. We will install yum-utils, device-mapper-persisten-data and lvm2.
2. Run `sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo` if you are installing docker community edition for [Centos](https://docs.docker.com/engine/install/centos/). 
3. Now run `sudo yum -y install docker-ce` to install docker.
4. Now we are going to enable the docker daemon by running `sudo systemctl enable --now docker`
5. Now we are going to configure out user without using sudo `sudo usermod -aG docker cloud_user`
6. We will need to add user to docker group by running `sudo usermod -aG docker cloud_user`. After running this command, we will need to log out by running `exit` and log back in to verify cloud_user added to docker group by running `groups`.
7. Now run `docker ps` to see status of your containers. No container will be shown since we dont have any.
8. We can try running `docker run hello-world`.



