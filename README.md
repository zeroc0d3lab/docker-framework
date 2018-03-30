# Docker Framework

Flexibility Configuration for Docker Environment. 
Distribution `alpine` docker container, use from [**Docker Alpine**](https://github.com/bhuisgen/docker-alpine).

## Environments
You can run docker-compose for different environment with selected containers
* Copy / Rename `.env.example` to `.env` file
  ```
  cp .env.example .env
  ```
* Change to execute script
  ```
  chmod a+x run_docker.sh
  ```
* Change environment in `run_docker.sh` file
  ```
  ENV="0"                      # (use: "development" or "production" as selected environment)
  CONTAINER_PRODUCTION="..."   # (selected containers will be run in production environment)
  CONTAINER_DEVELOPMENT="..."  # (selected containers will be run in development environment)
  ```
* Running script
  ```
  ./run.sh
  ```

## Documentation
* Configuration & How-To, see
[**Wiki Documentation**](https://github.com/zeroc0d3/docker-framework/wiki)

## Roadmap
* - [X] Multi Database Container & Multi Version Database
* - [X] Default Configuration NGINX (staging, staging-ssl, production, production-ssl)
* - [X] Healthy Check Docker Container
* - [ ] Unit Test Docker Container
* - [ ] Asynchronous / Background Job for Vulnerability Scan (Security Assessment)

## License
[**MIT License**](https://github.com/zeroc0d3/docker-Framework/blob/master/LICENSE)