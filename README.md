# node-docker-kubernetes-gcp
In this demo, we create a nodeJS demo app that uses the Express framework. 
We build the nodeJS app docker image and run it in a docker container to test it locally.

A GitHub Action job is used for CI/CD that builds and push the docker images to Docker Hub for future use 

## demo project 

[x] basic structure (controllers, models, routes)

[x] define entry point (app.js)

[x] install dependencies  (express, babel-cli, babel-preset, babel-preset-env, jest)

[x] add basic page and routes

### setup docker

[x] create dockerignore

[x] create dockerfile

[x] build docker image  (docker build . -t ..myDockerHubName../node-docker-kubernetes-gcp)

[x] run image (docker run --name nodeDemo -it -d -p 3000:3000 ....../..... see above)

### setup github actions for ci/cd and push image to docker hub

[x] add github action in repository

[x] create repository on dockerhub

[x] generate access token on dockerhub (settigs-security) 

[x] add action secrets (settings)

