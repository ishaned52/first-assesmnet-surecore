(Step 1)

===Docker==

Vid to Follow : https://youtu.be/3c-iBn73dDE

The above video should be enough to get started with docker and docker compose as it covers most of the theory points. 

To get comfortable with docker, please also do the following tasks as well.

1. A simple webserver with nginx
2. 

2.1 Get a small frontend from git (Ex :- https://github.com/creativetimofficial/material-dashboard-angular2)
2.2 Write a Dockerfile, build it and run it
2.3 Write a docker compose file to orchestrate it
2.4 Check container logs
2.5 Get inside the container exec and modify something (Ex :- create a new file/folder)

Notes :- Use a sepearate network, Use a non root user

3. 

3.1 Create a dockerhub account and create a private repository
3.2 Tag and push the previously built frontend to dockerhub

Notes :- Use an access token instead of the password

4.

4.1 Get a spring project from git (Ex :- https://github.com/sangqle/springboot-postgresql)
4.2 Deploy a postgresql database (using docker)
4.3 Containerize the application and write a docker compose file to orchestrate the deployment

Notes :- 

i. Place the application and the database in the same docker network.
ii. Experiment with docker volumes. Use a directory as a volume first and then use a named volume (Use permissions and access rights correctly ro, rw).
