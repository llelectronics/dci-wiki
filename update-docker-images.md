# Update docker images

For some reason updating the debianci images on dockerhub is not enough as there are some pangea/debian
images that are the actual docker images used by dci to build packages.

So ssh to the builders with "do-ssh-key-blue-private.pem" key and use docker to edit images
i.e.

`docker run -dit pangea/debian:2001 bash  
 docker exec -it <ID_from_above> bash  
 change stuff in container and exit out  
 docker commit <ID> pangea/debian:2001`


