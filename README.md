Dockerized HybridCheck Shiny App
================================

This is the Dockerized Shiny App for HybridCheck.

The image is available from [Docker Hub](https://registry.hub.docker.com/u/ward9250/dockerized-hybridcheckapp/).

## Usage:

To use this container you will need Docker installed on your computer.

To run this Shiny App container on your computer:

```sh
docker run --rm -p 80:80 ward9250/dockerized-hybridcheckapp
```

If you are on OS X or Windows operating systems you need to use
the command:

```sh
boot2docker ip
```

In order to find out the IP address of the Virtual Machine on your computer
that is running your docker containers. You then enter the IP address into
your webbrowser to load up an analysis session. If you are on Linux, then 
entering localhost as the address in your web browser should work.

## Intended purpose:

This container was created to avoid issues installing and running the R package
'HybridCheck', and its companion Shiny based web-app 'HybridCheckApp'. Common
issues installing and running these include different versions of R and R
packages, non-standard R library locations and so on.

If you learn Docker enough to use it to download and run containers, you avoid
all these possible pitfalls, as everything needed to get the package and
web-app running is provided for in this container, which will run on any system
Docker is available for, which certainly covers Windows, OS X, and the popular
GNU/Linux distros.
