
# Docker Notes


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
Remove all images ==>   docker rmi $(docker images -q)
======================================
