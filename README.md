# Getting started
This is the master installation file for GovA11y. You should be able to start this all easily from a the CLI. 

# Requirements
* Docker
* +32G of RAM

# Installation
Pull down git repository. Edit the `./docker/actors-only.yml` file

```
cd docker
docker network create --driver bridge --subnet=10.50.0.0/16 --ip-range=10.50.0.0/24 --gateway=10.50.0.1 --attachable --scope local gova11y
docker compose -f actors-only.yml up -d
```
