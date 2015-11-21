Neo 4j Scaffold
======
This is just mean to be a scaffold using docker, docker-compose and Neo4j. Once installed correctly you will have a neo4j instance running that you will be able to reach from your host machine.






Install
=====

1. If you are using a mac you can install many things. I perfer the old school docker osx. Why because it uses NFS and it super fast. Follow instructions here . https://github.com/nearhan/docker-osx

2. Install docker-compose

```
 brew install docker-compose 
```


Running
======

Great you have docker running on a linux container within your virtualbox. How do i use these things?

First open up your virtual and find the linux image. Open settings and go into system. Make you have given the VM about 4 gigs of memory.

Okay now you are ready to begin.

1. Run


```
	docker-osx shell
```

This will boot up the VM, and ssh you into that vagrant box. This script also maps the IP of your VM image to localdocker.  This will be important later.


2. Now run
 
```
   docker-compose up
```
This will read your docker-compose.yml file. Build all the containers and run their specfic cmd. 

In this instance you will download the offical neo4j image. Docker will then run this container. Expose ports 7474 so that you will be able to reach from the outside. And start the server.



3. If done correct you will be able to curl localdocker:7474



![stuff](https://raw.githubusercontent.com/Nearhan/gogoChess/master/assests/image.png)










