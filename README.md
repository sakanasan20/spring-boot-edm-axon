# spring-boot-edm-axon

## Run locally with ZIP file

__Download Axon Server__
- [Axon Server SE](https://docs.axoniq.io/reference-guide/axon-server/installation/local-installation/axon-server-se)

__Unzip file__

__Chang directory to unzip folder__

__Setup configuration (optional)__
* [configuration-properties](https://docs.axoniq.io/reference-guide/axon-server/administration/admin-configuration/configuration#configuration-properties)
* Add `config` folder
* Add `axonserver.properties` file
* Add `server.port=8024` in properties to setup port number
* Add `axoniq.axonserver.name=My Axon Server` in properties to setup server name
* Add `axoniq.axonserver.hostname=localhost` in properties to setup hostname name
* Add `axoniq.axonserver.devmode.enabled=true` in properties to enable develop mode

__Execute JAR__
- `java -jar axonserver.jar`

__Browse to dashboard__
- `http://localhost:8024`

## Run locally with Docker

__Install Docker__

__Create docker data folder__
* Create `docker-data` folder

__Setup configuration (optional)__
* [configuration-properties](https://docs.axoniq.io/reference-guide/axon-server/administration/admin-configuration/configuration#configuration-properties)
* Add `config` folder
* Add `axonserver.properties` file
* Add `server.port=8024` in properties to setup port number
* Add `axoniq.axonserver.name=My Axon Server` in properties to setup server name
* Add `axoniq.axonserver.hostname=localhost` in properties to setup hostname name
* Add `axoniq.axonserver.devmode.enabled=true` in properties to enable develop mode

__Run in cmd__
* `docker run --name axonserver -p 8024:8024 -p 8124:8124 -v "PATH_TO_YOUR_DOCKER_DATA_FOLDER/data":/data -v "PATH_TO_YOUR_DOCKER_DATA_FOLDER/eventdata":/eventdata -v "PATH_TO_YOUR_DOCKER_DATA_FOLDER/config":/config axoniq/axonserver`

## Run locally with Docker Compose

* [Running Axon Server in Docker - Continuing from local developer install to containerized](https://developer.axoniq.io/w/running-axon-server-in-docker-continuing-from-local-developer-install-to-containerized)

