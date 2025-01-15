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


# CHECK THE DOCKER VERSION
$ sudo docker version

# run a particular image inside the Container
$ sudo docker run <image_name> <container_name>

# Basic Docker Commands
# To run a Container
$ docker run <image/applicationname>
# To list all the running Containers
$ docker ps
$ docker ps -a (To see all the containers Stopped/Running)

# To Stop a Running Container
$ docker stop <containerID/ContainerName>

# To remove a started or stopped container permanently. 
$ docker rm <containerID/ContainerName>

# To see the list of images
$ docker images

# To Remove an image
$ docker rmi <imagename>

# To Download an image
$ docker pull <imagename>

# To Execute a command inside the docker container
$ docker exec <container_name> <command_to_execute>

# TO RUN THE CONTAINER IN THE DETACHED MODE. 
$ docker run -d <container_name>
