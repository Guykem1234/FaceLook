# FaceLook
 Social Network Using node.js & angular and sql for db
 
 
#### Set Up Project 
  - 1.) you need to install docker on your computer
  - 2.) create the server image: go the server folder open command line and run
```sh
  docker build -t server:v1 .
```
 - 3.) create the client image: go the client/FaceLook-front folder open command line and run
```sh
  npm install
```
```sh
  ng build --prod
```
```sh
  docker build -t facelookfront:v1 .
```
  - 4.) you need to create a sharable network env in docker by run:
```sh
  docker network create somenetwork
```
  - 5.) you need to create all the instances(containers) for elasticsearch, kibana, server, client, sql server, prometheus. this can be achieved by using the docker-compose file : 
```sh
  docker-conpose up
```
