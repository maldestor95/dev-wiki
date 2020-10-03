

# Powershell

* Remove all Exited container => `(docker ps -a |findstr Exited) | foreach-object {docker rm $_.split(" ")[-1]}`
* Buid a docker compose with a specific name    =>  `docker-compose --project-name SERVER -f ./docker-compose.dev.yml build`
* Run a docker compose with a specific name=>  `docker-compose --project-name SERVER -f ./docker-compose.dev.yml up`
* Dockerise an app with a specific dockerfile and a given name    =>  `docker build -f .\path\Dockerfile -t apptest .`
* Run the container =>  `docker run apptest`
