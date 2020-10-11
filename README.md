# Docker Services
This repository facilitates by providing services like databases (e.g postgres) in a containerized environment with one command.

It uses [Dokcer](https://docs.docker.com/get-started/overview/ "Docker overview") for containerization and [docker-compose](https://docs.docker.com/compose/ "Overview of Docker Compose") to manage these services.

- [Docker Services](#docker-services)
  - [Available Services](#available-services)
  - [Service Names](#service-names)
  - [How To?](#how-to)

## Available Services

- Postgres
- MSSQL Server

## Service Names

Followings are the exact name of the above [available services](#available-services). These names are required to run the service as described in the [How To?](#how-to) section.

- postgres
- sqlserver

## How To?
Make sure, you have [Docker](https://docs.docker.com/get-docker/ "Get Docker")  and [docker-compose](https://docs.docker.com/compose/install/ "Install Docker Compose") installed on your system.

1. Clone/Download this repository
2. Run `docker-compose up -d <service_name>`
   1. Here `<service_name>` is your required service. E.g for postgres, I'll run `docker-compose up -d postgres`
   2. If you dont know the exact name of your service then open the `docker-compose.yml` file and check the services section
   3. If you want to run all the services mentioned in the `docker-compose.yml` file then run `docker-compose up -d`
   4. `-d` is a flag to run container in the background. You can omit this flag if you want to know what is happening
