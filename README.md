# dev-ops-project

**On the road to be a Docker Captain :)**

Doing this project to learn some more about Docker, Docker-Compose and NGINX...


**Important considerations**

When use in production mode use the copy mode on the dockerfiles instead of volumes.

*Why?* The volume mode is to execute all the changes on your code in real time.

**To run this project:**

$ docker-compose up -d --build


**To clean all the docker trash :D**

$ sudo ./docker-clean.sh