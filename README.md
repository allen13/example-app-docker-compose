example-app-docker-compose
--------------------------

Run your app in docker compose

    docker-compose up

Run your app using docker stack, which will deploy either to docker swarm or kubernetes depending on how you have set up your docker engine.

    docker stack deploy --compose-file ./docker-compose.yml example-app

Navigate to localhost:5000 after either one has come up. These two approaches should be run independent from one another unless you change the conflicting port.

The kube folder contains kubernetes manifests harvested from the output of docker stack deploy.

