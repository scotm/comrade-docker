# Docker amd Compose Files for Comrade

The Dockerfile can be used to create a repeatable deployment environment for the [COMRADE](https://github.com/scotm/canvassing) canvasing suite by the Scottish Socialist Party.  The docker-compose.yml file automatically loads supporting containers (database and nginx), and configures these to support a new instance of COMRADE.

## Building:

    git clone https://github.com/scotm/canvassing.git comrade
    docker build -t leynos/comrade .

## Running:

Using docker-compose:

    docker-compose up

## To Do

Actually get the whole shebang running.

## Dependencies

This docker file was tested with Docker 1.3.1, but should work with any newer version.  Installation instructions can be found [here](https://docs.docker.com/installation/).

The compose file requires ```docker-compose``` which can be installed from [here](https://docs.docker.com/compose/install/).

I've so far done eveything using CentOS 7, but any 64-bit Linux distro supported by Docker will work.

## Copying

These config files are licensed as ISC, originally by Leynos, with the exception of the nginx config, which is licensed as CC-BY-NC-SA-4.0, originally by Digital Ocean (https://www.digitalocean.com/community/tutorials/how-to-deploy-python-wsgi-applications-using-uwsgi-web-server-with-nginx).
