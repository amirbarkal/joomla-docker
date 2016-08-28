[logo]: https://www.google.co.il/url?sa=i&rct=j&q=&esrc=s&source=images&cd=&cad=rja&uact=8&ved=0ahUKEwik8Men1eTOAhVEuxQKHanjDhcQjRwIBw&url=https%3A%2F%2Ffreshmail.com%2Fplugin%2Fjoomla-newsletter%2F&psig=AFQjCNE61bQO0GRTbAyhb8RXyF8s8o1nOA&ust=1472492803860490 "JOOMLA"

# Joomla + MySQL + phpMyAdmin on Docker. 
### Written by Amir Barkal

## Environment details:
- MySQL root password: 12345678
- Joomla database name: joomla
- MySQL hostname: mysql

# FAQ


## What is this?
A fast way to spin up joomla using Docker.

## How do I configure it?
1. Download and install [Docker](http://www.docker.com/products/docker#/windows)
2. Clone this repo
3. `cd joomla-docker`
4. `docker-compose.exe up`

## How do I access Joomla?
Open `http://DOCKER_HOST:80`

## How do I access phpMyAdmin?
Open `http://DOCKER_HOST:81`

## Where is my stuff?
Joomla and MySQL are mounted as docker volumes inside the `code` and `database `directories.

(Changes are persisted accross container restart \ removal)

## Can I bring my own stuff?
Yes.
Copy your website into the `./code` directory before starting the environment.

For example, if you have an Akeeba ZIP file, extract its content to `code` and run

`docker-compose up`

## Help! I need a different PHP/Joomla version!
Edit `docker-compose.yml` and change the joomla image [as per your requirements](https://hub.docker.com/_/joomla/).

## I'm having trouble installing Docker :-(
See if this video helps you:

#[![See if this video helps you](http://img.youtube.com/vi/S7NVloq0EBc/0.jpg)](http://www.youtube.com/watch?v=S7NVloq0EBc)
