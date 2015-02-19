Docker Joomla Apache server
======

This repository contains an image with Joomla's latest release based upon the gjong/apache docker image. It contains:

* Apache 2.x 
* PHP
* MySQL
* Joomla

##########################
## Getting the container##
##########################

You can get the image by running, this will install this image into your local docker repository.

```
docker pull vints24/Apache-Joomla_V3-Docker
```

##########################
## Running the container##
##########################

When the container starts it will automatically start the Apache webserver with Joomla installation and MySQL. The Apache server 
will be running on port 80, which is also exposed out of the container.

You can run the container with access to the webserver by running:

```
docker run -d -p 80:80 vints24/Apache-Joomla_V3-Docker
```

Once the container is running you will get a joomla website on : http://localhost/ 
That still needs to be configured using the installation script. 
The password for the database is left blank, so you can create the Joomla website easily.
