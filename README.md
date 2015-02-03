[![Docker Build Status](https://circleci.com/gh/htmlgraphic/Docker/tree/develop.svg?style=svg&circle-token=b51ac0eded585009395fde219719b0c86f5320d2)](https://circleci.com/gh/htmlgraphic/Docker/tree/master)

##Quick Start
```bash
    $ git clone https://github.com/htmlgraphic/Docker.git && cd Docker
    $ cd Docker/Apache
    $ make
    $ make build
```

If you found this repo you are probably looking into Docker or already have knowledge as to what Docker can help you with. In this repo you will find a number of complete Dockerfile builds used in **development** and **production** environments. Listed below are the types of systems available and an explanation of each file. 

* Docker is a containerization system that utilized LXC known as Linux containers, uses kernel names pacing a cgroups in order to isolate processes.
* Docker containers can run side-by-side with other containers, but act as an individual server.

###Repo Breakdown
* [**CoreOS**](https://github.com/htmlgraphic/CoreOS) - Scripts used for the loading of services into Fleet managing Docker containers on CoreOS
* [**Docker**](https://github.com/htmlgraphic/Docker) - Build scripts the creation of my different types of servers. 


---

#####[Apache Web Server](https://github.com/htmlgraphic/Apache)

#####Base Container
* A base container used by other builds to make the creation process faster

#####Data Container
* Files and data for Apache is stored here 

#####[Postfix Mail Server](https://github.com/htmlgraphic/Postfix)

#####MySQL server
* `make build`
* `make run` create a stateless data container and start a MySQL instance storing data on the simple **Busybox** data container


##Build Tests
As you continue to build more containers and extend functions, a very useful tool is using a *test driven development* solution. This repo is setup to use [CircleCI](https://circleci.com/gh/htmlgraphic/Docker) and have numerous tests set within `circle.yml`. It is very good to know that your built containers pass all the tests you define before setup in production.

As each Docker container is split into its own repo deeper tests and master builds will be managed via a build a deployment service called [Shippable](http://shippable.com)
