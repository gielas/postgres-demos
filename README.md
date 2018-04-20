# Postgres Docker Demo

## Requirements

[Docker](https://docker.com),
[Docker for Windows](https://www.docker.com/docker-windows) or 
[Docker for Mac](https://www.docker.com/docker-mac)

## Getting Started

To start a local development environment run ```docker-compose up```. This starts all services.

## postgres

An example script in the [db](db/) folder is executed to populate the database. Scripts placed in this folder will be executed in alphabetical order.

The database is persisted between restarts. To recreate the database volume and rerun database creation scripts add the -V parameter: ```docker-compose up -V postgres```.

## pgadmin

Go to http://localhost:5050/ and login as _postgres_ with password _postgres_.

Click on Add New Server to connect to the postgres instance. Use Host name _postgres_, Username _postgres_ and Password _postgres_.

See [docker-compose.yml](docker-compose.yml).
