# Docker

Docker Images : 
```
Packages Template or a plan of the application. 
We can create our own images and push it to docker repository. 
```

#### Getting Started with Docker
```
Docker has two editions
o	Community edition
o	Enterprise Edition. 
```
```
Docker is available for the below operating systems 
o	Linux
o	Windows
o	MAC
o	Cloud platforms like AWS , Azure etc..
```

## Installing Docker
1. Navigate to the below url <br>
[Docker](https://docs.docker.com "Docker")

2. Click on Get Docker.

3. Uninstall any older versions of the docker using the below command. <br>
$ sudo apt-get remove docker docker-engine docker.io containerd runc

4. Then install docker using the commands for a particular operating system. <br>
Once the Installation is successful we can version the version of the docker using 
$ sudo docker version


#### Check the Docker Version:
```
$ sudo docker version
```
#### Run a particular image inside the container:
$ sudo docker run <image_name> <container_name>

### Basic Docker Commands:
#### To Run a Container:
$ docker run <image/applicationname>

#### To List All the Running Containers:
$ docker ps
$ docker ps -a (To see all the containers Stopped/Running)

#### To Stop a Running Container:
$ docker stop <containerID/ContainerName>

#### To Remove a Started or Stopped Container:  
$ docker rm <containerID/ContainerName>

#### To See list of the Docker images:
$ docker images

#### To Remove an Image:
$ docker rmi <imagename>

#### To Download an Image:
$ docker pull <imagename>

#### To Execute the Command inside the docker container: 
$ docker exec <container_name> <command_to_execute> <br>

#### To run the Container in detached mode: 
$ docker run -d <container_name>

#### To Attach a detached container: 
$ docker attach <first_five_letters_container>

#### To login into Docker container in interactive mode.
$ docker run -it <image_name> bash

#### To Make the container run for a specific amount of time
$ docker run <image_name> sleep 20

#### To login into a container and run a command
$ docker exec <container_id> <command>

#### To run a specific container and give a name
$ docker run --name <container_name> -d <imagename>

#### To remove all the images
$ docker rmi $(docker images -q)

#### Assigning tags for Containers
$ docker run <image_name>:<tag> 

#### To run the Container in the Interactive mode
$ docker run -i <image_name>

#### Port Mapping a Container.
$ docker run -p <new_port>:<port_to_map> <image_name> <br>
$ docker run -p 80:5000 redis

#### To preserve the data inside the container we do volume mapping
$ docker run -v <new_directory>:<directory_to_be_mapped> <image_name>

#### To View the logs of the Container
$ docker logs <container_name>

#### To run a docker container and get information about the container
$ docker run <container_name> <command_to_get_the_information> <br>
$ docker run ubuntu cat /etc/*release* <br>
$ docker run <container_name>:tag <command_to_get_the_information> <br>
$ docker run ubuntu:17.10 cat /etc/*release* <br>

#### To get the Information about the docker container like IP and other details 
$ docker inspect <container_id>
