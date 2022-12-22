- Docker registry images.
- https://hub.docker.com/repository/docker/mabeatti/contacts-app-ui
- https://hub.docker.com/repository/docker/mabeatti/contacts-app

== Generate Docker Image

- Generate a Docker image:

./mvnw spring-boot:build-image -Dspring-boot.build-image.imageName=<you-id>/contacts-app:v1

- Push image

docker tag contacts-app mabeatti/contacts-app:v1.0

docker push mabeatti/contacts-app:v1

== Creating a Kubernetes deployment
