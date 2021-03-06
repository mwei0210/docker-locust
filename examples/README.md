This folder contains a few examples of running locust docker images (using docker compose).

They include:
* running standalone node of locust 
* running distributed locust cluster
* running distributed locust cluster without web ui with timed execution

The examples use a simple [locustfile](locust-scripts) that issues HTTP GET '/' requests and logs some information.

To run relevant examples use docker-compose, for example:
```
docker-compose -f docker-compose-standalone.yml up
```
or:
```
docker-compose -f docker-compose-distributed.yml up
```
or:
```
docker-compose -f docker-compose-distributed-headless.yml up
```


To shut down example nodes use:
```
docker-compose -f docker-compose-standalone.yml down
```
or:
```
docker-compose -f docker-compose-distributed.yml down
```
or:
```
docker-compose -f docker-compose-distributed-headless.yml down
```