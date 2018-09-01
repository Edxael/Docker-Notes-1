
# Docker Notes

## Main Documentation site: 
### https://docs.docker.com/


=================================================
## Mini Tuts to see: 

-|- Docker with Node.js in 5-minutes
https://www.youtube.com/watch?v=edPrPcgjTgw

-|- Node.js - Create and deploy a microservice in less than 10 minutes using the micro framework
https://www.youtube.com/watch?v=dfvBrd6OeEo

-|- Creating a Docker container for a Nodejs + Expressjs + Mongo application - Tutorial
https://www.youtube.com/watch?v=0w0lJn4O6YQ


    - - - - - - - - - - - - - - - 

-|- Learn Docker in 12 Minutes (Full Code component creation)
https://www.youtube.com/watch?v=YFl2mCHdv24

-|- Docker Compose in 12 Minutes
https://www.youtube.com/watch?v=Qw9zlE3t8Ko


    - - - - - - - - - - - - - - - 

-|- Mini docker explanation ( 16 min code along )
https://www.youtube.com/watch?v=JprTjTViaEA

https://www.youtube.com/watch?v=wxxigbHwDGM



    - -[ PostgreSQL ]- - - - - - - - - - - - -

-|- Docker and Postgres in 10 Minutes
https://www.youtube.com/watch?v=aHbE3pTyG-Q

-|- Docker Compose Node.js, Redis, and PostgreSQL
https://www.youtube.com/watch?v=aetqo2nkQcA

-|- PostgreSQL and Docker - getting started
https://www.youtube.com/watch?v=A8dErdDMqb0




-|- docker-compose Tutorial
https://www.youtube.com/watch?v=A0nhB8YASgw

Easy Docker Dev to Production Setup for Small Projects
https://www.youtube.com/watch?v=LSyIE-bTt5U


    - - - - - - - - - - - - - - - 

-|- YAML | In One Video
https://www.youtube.com/watch?v=cdLNKUoMc6c
https://www.youtube.com/watch?v=gIxLDYvfGcQ


=================================================

  


** Terminal:
docker container run --publish 80:80 nginx
    or
docker container run --publish 80:80 --detach nginx

** Browser:
http://localhost/
--> Welcome to nginx!
If you see this page, the nginx web server is successfully installed and working...


** Terminal:
docker container stop


======================================
             Handy Commands
======================================
List all containers (only IDs)==>   docker ps -aq
Stop all running containers ==>  docker stop $(docker ps -aq)
Remove all containers ==>   docker rm $(docker ps -aq)
Remove a running container ==>   docker container rm -f <ContainerName>
Remove all images ==>   docker rmi $(docker images -q)
======================================


run a container with a bash terminal to access inside of the container: 
    Edxael: docker container run -it --name myproxy nginx bash
    root@64e1880a583c:/#

Use command "exit" but this command will also stop the container. 

Another way to achieve this and be able to exit without stoping the container: 
    use the exec 