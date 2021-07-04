# Dockerizing-Drupal-IITBx
Dockerizing Drupal using  drupal version 9.2.0 and php version 7.4

## Installation

### Basic Setup
* Install [Docker](https://docs.docker.com/get-docker/) and [docker-compose](https://docs.docker.com/compose/install/). Make sure that you install both of them specific to your OS and version (Linux, Windows, Mac)
* ```git clone https://github.com/fresearchgroup/Dockerizing-Drupal-IITBx.git```
* ```cd Dockerizing-Drupal-IITBx```
* ```sudo docker-compose -f docker-compose.yml --env-file .env up```
* Note IP Address of MySQL docker container
  * ```sudo docker ps```
  * ```sudo docker inspect <ContainerID_MySQL>```

### Drupal
* Once, the docker is up and running, browse ```localhost``` on your browser
* Choose language: English
* Choose profile: Standard
* Database Configuration
  * Database type: MySQL
  * Database name: drupal
  * Database username: user
  * Database password: password
  * Advanced options, Host: IP Address of MySQL docker container 
* Mention site details (name, admin username and password, etc.) 

### Other important commands
* Find list of dockers running: ```sudo docker ps -a```
* Go into a docker container: ```sudo docker exec -it <ContainerID> /bin/bash```
* Stop a docker container: ```sudo docker stop <ContainerID>```
* Remove a docker container: ```sudo docker rm <ContainerID>```




