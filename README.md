Notes

\# Merge Request

Git stash - store temporarily

git checkout -b \- new branch

Git checkout | git switch \- switch branch

Git branch - list branch

Git pull - fetch and integrate changes from remote

npm i - install npm

Git stash apply - apply the most recent stashed changes

Git commit -m “” - comit

Git push - push changes

\# Docker

Build: docker build -t .

Run: docker run -it --rm

Containers:

docker ps:list container

docker ps -a: list container

docker stop

docker container ls: list container

docker rm :Remove Container

Image:

docker image ls: list images

docker run —rm -it : run image

docker run -it /bin/bash : get into shell

docker rmi : Remove Docker Image

Logs: docker logs

Clean all docker stuff: sudo docker prune -

\# Docker Compose

docker-compose build: Builds Docker images based on the Dockerfile in the current directory.

docker-compose up -d: Starts containers defined in the Docker Compose file in detached mode (in the background).

docker-compose down: Stops and removes containers defined in the Docker Compose file.

docker volume ls: list all mounted volumes

docker volume inspect : inspect volume to see mount point

\# Docker MongoDB

Shell: sudo docker exec -it mongodb mongosh -u admin -p password

IP: sudo docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}'

\# Keygen

ssh-keygen -t rsa -b 4096 -C “shiva.c@breachlock.com"

\# Mongo

show dbs

use

show collections

db..find().limit(10)

db..countDocuments()

\# Linux

netstat -tuln

ps aux

\# VI

“i”: insert on the left side of cursor

“a”: append on the right side of the cursor

“o”: Insert a new line below

0 : beginning of the line

$: end of the line

Shift + G: end of file

gg: top of file

Next world: w | (jumping by spaces): Shift + w

Previous word: b

Find in the line (right of cursor): f

(left of cursor): Shift + F

Ctrl + d: scroll down

Ctrl + u: scroll up

Shift + i: insert at the beginning of the line

Shift + a: insert at the end of the line

Shift + o: create a line above and prepare insert on next line

arrow / w / b: to jump number of lines or word

Shift+G: go to line | Control + o: to go back to the same from where we jumped

dd: delete line

d: next n lines

%d: delete all lines

y: copy

p: paste deleted

u: undo

Ctrl + r: redo

Visual mode: v

Command mode:

:/

: n for next / Shift+N to previous match

:%s///g: /g for global, and not only for line
