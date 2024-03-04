# Columnar test IRIS internal
The package creates a very basic IRIS instance in Docker    
the code is also available in IPD
## Description
+ The idea of this package is to compare performance of columnar storage   
inside IRIS without wrapping it to some foreign platform that is not my world
* In addition I do not want to measure nework performance between 2 containers,
but inside a closed IRIS environment that I have full under my control
* Even the use of SMP or some other browser based presentation has some
* influence that I want to avoid. Measuring should be as close to the core as possible. 
### Prerequisites
Make sure you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Docker desktop](https://www.docker.com/products/docker-desktop) installed.
### Installation
Clone/git pull the repo into any local directory
```
$ git clone https://github.com/rcemper/Columnar-IRIS-internal.git
```
To build and start the container run:
```
$ docker compose up -d && docker compose logs -f
```
To open IRIS Terminal do:
```
$ docker-compose exec iris iris session iris
USER>
```
or using **WebTerminal**
```
http://localhost:42773/terminal/
```
To access IRIS System Management Portal
```
http://localhost:42773/csp/sys/UtilHome.csp
```
### How to use it
All tests are running in Namespace USER and are initiated    
exclusively from command prompt. 
