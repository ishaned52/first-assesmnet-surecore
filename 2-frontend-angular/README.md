# Task 2: Angular Frontend

https://github.com/creativetimofficial/material-dashboard-angular2

create docker image
----------------------

docker build -t angular-dashboard . 

run the container
------------------
docker run --name docker-container -p 4200:4200 angular-dashboard

run the composer
------------------
docker composer up


check docker logs
------------------

docker logs docker container


change inside with exec
-----------------

docker exec -it angular-container sh

cd /app
mkdir new-folder
touch hello.txt
echo "Hi from inside the container" > hello.txt

ls -l
cat hello.txt

quit          -  exit

 Verify from outside

 docker exec -it angular-container ls /app
docker exec -it angular-container cat /app/hello.txt



Run in a custom docker network
----------------------------------

docker network create my-first-network

docker run --name docker-container-2 --rm -p 4200:4200 --network my-first-network angular2


Use non root user 
--------------------

