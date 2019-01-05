# docker-odoo-pg
Dockerfile for Odoo on PostgreSQL


## Uses

 * [Docker Engine 1.13.0+](https://www.docker.com/get-started) (for docker-compose 3)
 * [Odoo 12.0](https://hub.docker.com/_/odoo/)
 * [Postgresql 11.1 (alpine)](https://hub.docker.com/_/postgres/)

## Instructions

You can set the following environment variables:

 * `PGUSER` for the Postgres username (default: `odoo`)
 * `PGPASSWORD` for the Postgres password (default: `myodoo`)

### Usage

Go where your `docker-compose.yml` is and run:

    docker-compose up -d
 
## Resource limitations

### Odoo

 * Memory limit: 1GB
 * Memory reservation: 50MB
 * CPUs: 0.5
 * CPUs reservation: 0.1

### PostgreSQL

 * Memory limit: 1GB
 * Memory reservation: 50MB
 * CPUs: 0.5
 * CPUs reservation: 0.1
