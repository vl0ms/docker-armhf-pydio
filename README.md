# docker-armhf-pydio
Pydio is like Google Drive for your personal cloud. 
This repository allows you to run Pydio on your ARMv7 device with Docker. This includes a built in MySQL server for an easy setup.

# how to pull:
docker pull vl0ms/armhf-pydio

# how to build:
docker build -t vl0ms/armhf-pydio

#how to start:
docker run --name=pydio --restart=always -it -d -p 80:80 -p 443:443 -v /your/data/files/:/pydio-data/files/ -v /your/personal:/pydio-data/personal/ vl0ms/armhf-pydio

# mysql parameters:
    url : localhost
    database name : pydio
    user name : pydio
    user password : pydio


P.S. You must ensure your host folder is accessable to the user with the uid 1000.
