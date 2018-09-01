
# Docker Notes

## Main Documentation site: 
### https://docs.docker.com/


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