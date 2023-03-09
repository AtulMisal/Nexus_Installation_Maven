# Nexus_Installation_Maven
Here with the help of maven we will install nexus and use to store our artifacts.

# We can install Nexus by two methods --
  1. By Installing nexus on server using all steps as in above.
  2. By using docker image.
  
 By docker image we will pull one nexus image for this we need to install docker on that system.
    1.apt update
    2.apt install docker.io
    3.docker pull sonatype/nexus3:latest
    4.By this one image will be pulled 
    5.docker image ls    -- will list the image with id
    6.Now we have to create one container from this image.
    7.docker container run -itd --name=Nexus -p 8081:8081 image_id ----get it from step 5
    8.docker container ls -- will show running cotainer 
    9. now open port 8081 with ip of that server as ip:8081
    10.It will ask password which is present inside container
    11.docker exec -it container_id /bin/bash    --- will go inside container
    12. ls
    13.cd nexus*
    14.Check here one file with password*  cat that file
    
  
