# node-docker-kubernetes-gcp

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

### add kubernetes

[x] create deploy.yml

### gcp

[x] authenticate -> gcloud auth application-default login
[x] initialize new project - gcloud init
[x] enable services: ?????
 gcloud services enable servicemanagement.googleapis.com servicecontrol.googleapis.com cloudresourcemanager.googleapis.com compute.googleapis.com container.googleapis.com containerregistry.googleapis.com cloudbuild.googleapis.com
[x] create main.tf and providers.tf
[x] initialize terraform -> terraform init  (had to brew install terraform)
[x] create resources -> terraform apply -auto-approve
[x] connect to the cluster -> gcloud container clusters get-credentials <clustername>
[x] run kubernetes deployment
    kubectl apply -f <yourDeploy.yml file>
    kubectl get all         # view al the kubernetes resources
    kubectl get nodes       # view nodes
    kubectl get pods        # view pods
    kubectl get services    # view services
    kubectl get events      # view all event in the clust   
