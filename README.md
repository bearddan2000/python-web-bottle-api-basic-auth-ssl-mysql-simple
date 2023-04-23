# python-web-bottle-api-basic-auth-ssl-mysql-simple

## Description
Simple web app that serves static pages
for a bottle project.

Uses sqlalchemy query a table `dog`.

Is self-signed ssl cert.
Requires basic authentication for endpoints.

| username | password |
| -------- | -------- |
| *user* | *pass* |

## Tech stack
- python
  - bottle
  - sqlalchemy
  - cheroot
- bootstrap
- jquery
- dataTable
- mariadb
- ssl

## Docker stack
- alpine:edge
- python:latest
- mariadb:latest

## To run
`sudo ./install.sh -u`
- Endpoint
  - curl -i -k https://localhost/dog -u 'user:pass'

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
- [Bottle sqlalchemy setup](https://github.com/iurisilvio/bottle-sqlalchemy/blob/master/examples/basic.py)
- [Disable ssl for testing](https://stackoverflow.com/questions/23013220/max-retries-exceeded-with-url-in-requests)