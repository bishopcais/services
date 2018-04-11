cir-services
============

**Last Updated**: 04/11/2018

Repository to host the necessary scripts to run the containers that house services necessary for the CIR, but are
not being developed by us for the CIR (which are all in their own repos). Each service should be bounded to a 
minor version (x.x), but in some cases, we may need to further bind it to a specific bugfix (x.x.x). We should
strive to keep all services relatively up-to-date when possible. Whenever a change is made, please update the
date above and the version below of what got changed.

Using this repo requires [docker](http://docker.com) and [docker-compose](https://docs.docker.com/compose) to be
installed.

Use `docker-compose [up|down|start|stop|restart]` as necessary for running things (you most likely want to use `-d`
with `[up|start|restart]` to remain detached from the containers output unless you're debugging something).

Current Services
----------------
* [RabbitMQ](http://rabbitmq.com): 3.7
* [Redis](https://redis.io/): 4.0
* [MongoDB](https://www.mongodb.com/): 3.6
* [PostgreSQL](https://www.postgresql.org/): 10.3
