Dockerized HybridCheck Shiny App
================================

This is the Dockerized Shiny App for [HybridCheck](http://ward9250.github.io/HybridCheck/index.html)

The image is available from [Docker Hub](https://registry.hub.docker.com/u/ward9250/hybridcheckapp/).

## Usage:

To run this Shiny App on your computer:

```sh
docker run --rm -p 80:80 ward9250/hybridcheckapp
```

and it will avaliable at http://127.0.0.1/ or http://localhost

Remember that if you are on OS X or Windows operating systems you need to use the command:

```sh
boot2docker ip
```

In order to find out the IP address of the Virtual Machine on your computer that is running your docker containers. Then, instead of putting http://127.9.0.1/ or http://localhost into your web-browser, enter the
IP address that was returned by the command.

## Intended purpose:

This container was created to avoid issues installing and running the R package 'HybridCheck', and its
companion Shiny based web-app 'HybridCheckApp'. Common issues installing and running these include
different versions of R or R packages, non-standard R library locations and so on.

If you learn Docker enough to use it to download and run containers, you avoid all these possible pitfalls,
as everything needed to get the package and web-app running is provided for in this container, which will run
on any system Docker is available for, which certainly coveres Windows, OS X, and the popular GNU/Linux distros.
