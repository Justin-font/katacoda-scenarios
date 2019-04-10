This is your first step.
#Intro
You should run docker in sudo, but for this tuto we will do thing in root les mode (without sudo)
Warnning on your machine running docker without sudo iis higly unrecomander for security purpose
#Container 
## First step ubuntu container
- create a _ubuntu_ **container** from by running :
- `docker run -ti ubuntu`{{execute}}.
- now you are in the ubuntu container
- lets intall python : `apt-get update; apt-get install curl`{{execute}} then `Y`{{execute}}. 
- Now start python :`python`{{execute}} .
- Print Datamaran:`print('datamaran')`{{execute}} .
- exit from python:  `exit()`{{execute}} .
- exit from the container : `exit()`{{execute}} .

## Ubuntu and then install python? i don't need it 
It make more sens to create a python container !
- create a python conatainer: ` docker run -ti python `{{execute}} .
- Print Datamaran:`print('datamaran')`{{execute}} .
- exit from python (and the container btw):  `exit()`{{execute}} .

## woaw without instaling python i can run python !
And you can run more than pyhton, node, mongoDB, almost every tech have it own image and you can also create your own.
Here you can see all images avaible on Docker https://hub.docker.com/search?q=&type=image
