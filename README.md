cir-services
============

Repository to host the necessary scripts to run the containers that house services necessary for the CAIS,
but are not being developed by us for the CAIS (which are all in their own repos). Each service should be
bounded to a minor version (x.x), but in some cases, we may need to further bind it to a specific bugfix
(x.x.x). We should strive to keep all services relatively up-to-date when possible. Whenever a change is
made, please update the date above and the version below of what got changed.

Using this repo requires [docker](http://docker.com) and [docker-compose](https://docs.docker.com/compose)
to be installed.

Use `docker-compose [up|down|start|stop|restart]` as necessary for running things (you most likely want to
use `-d` with `[up|start|restart]` to remain detached from the containers output unless you're debugging
something).

Current Services
----------------
* [RabbitMQ](http://rabbitmq.com): 3.8
* [Redis](https://redis.io/): 5
* [MongoDB](https://www.mongodb.com/): 4.2
* [PostgreSQL](https://www.postgresql.org/): 10.3 (disabled)
