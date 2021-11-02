# crowsnest

"Elevator pitch - TODO"

This repository is the main repository of crowsnest. It contains examples of docker-compose setups:
* `docker-compose.base.yml` - defines the base services needed for getting up and running
* `docker-compose.auth.yml` - defines the additional config required to get authentication/authorization going

The compose files build on each other according to the principles outlined [here](https://docs.docker.com/compose/extends/#multiple-compose-files). As such, the following `docker-compose` commands are all valid:
* `docker-compose -f docker-compose.base.yml up`
* `docker-compose -f docker-compose.base.yml -f docker-compose.auth.yml up`
