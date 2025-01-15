# Docker
Docker
Docker Images : 
-	Packages Template or a plan of the application. 
-	We can create our own images and push it to docker repository. 

# GETTING STARTED WITH DOCKER. 
-	Docker has two editions
o	Community edition
o	Enterprise Edition. 
-	Docker is available for the below operating systems 
o	Linux
o	Windows
o	MAC
o	Cloud platforms like AWS , Azure etc..

# INSTALLING DOCKER
-	Navigate to the below url 
https://docs.docker.com
-	Click on Get Docker. 
-	Uninstall any older versions of the docker using the below command. 
$ sudo apt-get remove docker docker-engine docker.io containerd runc
-	Then install docker using the commands for a particular operating system. 
-	Once the Installation is successful we can version the version of the docker using 
$ sudo docker version


####CHECK THE DOCKER VERSION#### 
----------------------------
$ sudo docker version

#### RUN A PARTICULAR IMAGE INSIDE A CONTAINER
$ sudo docker run <image_name> <container_name>

### BASIC DOCKER COMMANDS
#### TO RUN A CONTAINER
$ docker run <image/applicationname>

#### TO LIST ALL THE RUNNING CONTAINERS
$ docker ps
$ docker ps -a (To see all the containers Stopped/Running)

#### TO STOP A RUNNING CONTAINER
$ docker stop <containerID/ContainerName>

#### TO REMOVE A STARTED OR STOPPED CONTAINER.  
$ docker rm <containerID/ContainerName>

#### TO SEE THE LIST OF DOCKER IMAGES
$ docker images

#### TO REMOVE AN IMAGE
$ docker rmi <imagename>

#### TO DOWNLOAD AN IMAGE
$ docker pull <imagename>

#### TO EXECUTE THE COMMAND INSIDE THE DOCKER CONTAINER. 
$ docker exec <container_name> <command_to_execute>

#### TO RUN THE CONTAINER IN THE DETACHED MODE. 
$ docker run -d <container_name>
