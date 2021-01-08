# docker-apache-server-example
Example of creation of a Docker image to run an Apache Web Server.

To build the Dockerfile and create a new image use :

    docker build -t="mywebserver" 

To create a container from the newly created image use:

    docker run -d -p 80:80 mywebserver

A container running an instance of our own Apache image is now running in detach mode and is now exposed at `<your-docker-host-ip>:80` (for instance `192.168.99.100:80`).

Go see the result in your browser.
