# Steps to follow for easy testing on local mac 

* docker pull node --> we need this image for testing
* go to whereever this code lives, hopefully you're already there :)
* docker run --rm --name test -v (pwd):'/test' -p 8080:8080 -it node bash
* now you're in the docker container, cd to /test and run npm start  
* Whatever you change will be reflected inside the docker container

# NOTES

<i> lsblk doesn't exist on macOS, also we want to do testing on a linux machine. If you're using a Linux machine no need to run this inside a docker container.

When we get the cloud credentials, we need to test this again on the cloud machine but this time without using docker.