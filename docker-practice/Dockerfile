# bring in base image
FROM ubuntu
# used to run a command
RUN apt-get install -y jenkins
# similar to run but used for executing a specific command. Unlike RUN
# it is not executed during build, but when a container is instantiated
# using the image being built
CMD "echo" "welcome to the docker file"
# overwrites CMD command, first command to be executed
ENTRYPOINT echo "overwrites CMD command"
# copies files in one particular directory to another directory
# from host to container
ADD /my_app_folder /my_app_folder
# environment variable 
ENV SERVER_WORKS 4
# where you would like to execute CMD commands inside of the container. 
WORKDIR /path WORKDIR ~/
# the application is active on this port number inside of the container
# specific to your container and only use inside of your container.
EXPOSE 8080
