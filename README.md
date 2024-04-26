Notes

# Merge Request
Git stash - store temporarily
git checkout -b <branch_name> - new branch
Git checkout <branch_name> | git switch <branch_name> - switch branch
Git branch - list branch
Git pull - fetch and integrate changes from remote
npm i - install npm 
Git stash apply - apply the most recent stashed changes
Git commit -m “<Message>” - comit
Git push - push changes



# Docker
Build: docker build -t <tag> .
Run: docker run -it --rm <tag>
Containers: 
	docker ps	:	list container
	docker ps -a		:  	list container
	docker stop <container_name>
	docker container ls	: 	list container	
	docker rm <container_id> 	:	Remove Container 
Image:
	docker image ls	: 	list images
	docker run —rm -it <IMAGE_NAME> 		: 	run image
	docker run -it <IMAGE_ID> /bin/bash 	: 	get into shell
	docker rmi <tag> 		:	 Remove Docker Image 

Logs: docker logs <container_id>
Clean all docker stuff: sudo docker <system / image / ..> prune -

# Docker Compose
docker-compose build		: Builds Docker images based on the Dockerfile in the current directory.
docker-compose up -d		: Starts containers defined in the Docker Compose file in detached mode (in the background).
docker-compose down		: Stops and removes containers defined in the Docker Compose file.

docker volume ls	: 	list all mounted volumes
docker volume inspect <volume_name>	: 	inspect volume to see mount point

# Docker MongoDB
Shell: sudo docker exec -it mongodb mongosh -u admin -p password
IP: sudo docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' <contier id>


# Keygen
ssh-keygen -t rsa -b 4096 -C “shiva.c@breachlock.com"



# Mongo
show dbs
use <db_name>
show collections
db.<collection>.find().limit(10)
db.<collection>.countDocuments()



# Linux
netstat -tuln
ps aux



# VI
“i”: insert on the left side of cursor
“a”: append on the right side of the cursor
“o”: Insert a new line below

0 : beginning of the line
$: end of the line

Shift + G: end of file
gg: top of file

Next world: w | (jumping by spaces): Shift + w
Previous word: b
Find <something> in the line (right of cursor): f <something>
	(left of cursor): Shift + F <something>

Ctrl + d: scroll down
Ctrl + u: scroll up

Shift + i: insert at the beginning of the line
Shift + a: insert at the end of the line
Shift + o: create a line above and prepare insert on next line

<number> arrow / w / b: to jump number of lines or word

<number> Shift+G: go to line | Control + o: to go back to the same from where we jumped

dd: delete line
<number> d: next n lines
%d: delete all lines

y: copy
p: paste deleted

u: undo
Ctrl + r: redo
 
Visual mode: v

Command mode:
:/<search keyword>		: n for next / Shift+N to previous match
:%s/<find>/<replace>/g	: /g for global, and not only for line
