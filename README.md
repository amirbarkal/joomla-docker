# Joomla docker-compose
### Written by Amir Barkal

## What is this?
   A fast way to spin up joomla using Docker.

## How to configure it?
1. Download and install Docker
2. Clone this repo
3. `cd joomla-docker`
4. `docker-compose.exe up`

## How to access Joomla?
Open `http://DOCKER_HOST:80`

## How to access phpMyAdmin?
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
Edit docker-compose.yml and change the joomla image as per your requirements.
