## Quick Start
```bash
    $ git clone https://github.com/htmlgraphic/Docker.git && cd Docker
    $ git submodule update --init --recursive
    $ cd Docker/Apache
    $ make
    $ make run
    $ docker ps
```
**After running the following commands you will see a working Apache & MySQL service.**

If you found this repo you are probably looking into Docker or already have knowledge as to what Docker can help you with. In this repo you will find a number of complete Dockerfile builds used in **development** and **production** environments. Listed below are the types of systems available and an explanation of each file. 


## Repo Breakdown
* Build scripts the creation of my different types of servers. [View all repos](https://github.com/htmlgraphic/Docker/tree/master/Docker)


---

#### Apache Web Service
* A web service instance to use for local development or production. [View updated repo](https://github.com/htmlgraphic/Apache#quick-start)

#### Base Container
* A base container used by other builds to make the creation process faster. [View layers of container](https://microbadger.com/images/htmlgraphic/base)

#### Postfix Mail Service
* A mail courier service created to help queue outgoing email from web servers. [View updated repo](https://github.com/htmlgraphic/Postfix#quick-start)

#### MySQL Service
* `make build`
* `make run` create a stateless data container and start a MySQL instance storing data on a simple **Busybox** data container. [View updated repo](https://github.com/htmlgraphic/MySQL/tree/mysql-server/5.7)

