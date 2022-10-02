# Deploy Laravel and React App to AWS ECS

## Requirements
* AWS Account

## Prerequisites
* Generate key pair in EC2 > Network & Security > Key Pairs > Create key pair

## How to deploy
1. Create RDS using [RDS Stack Script](https://github.com/theadonata/laravel-aws-deploy/blob/main/cloud-formation-template/rds/test-rds.yml)
2. Create these parameters in AWS SSM Parameter Store
  ![image](https://user-images.githubusercontent.com/13175937/193450091-1c3526c8-d31a-45ab-9cf1-b3ab4e01687f.png)
2. Create ECS Cluster using [ECS Stack](https://github.com/theadonata/laravel-aws-deploy/blob/main/cloud-formation-template/ecs-cluster/test-ecs.yml)
3. Deploy Backend using [Backend Stack](https://github.com/theadonata/laravel-aws-deploy/blob/main/cloud-formation-template/backend/test-backend.yml)
4. Deploy Frontend using [Frontend Stack](https://github.com/theadonata/laravel-aws-deploy/blob/main/cloud-formation-template/frontend/test-frontend.yml)

## Sources
* Frontend docker image [React Docker Image](https://hub.docker.com/repository/docker/theadonata/react-fe)
* Backend docker image [Laravel Docker Image](https://hub.docker.com/repository/docker/theadonata/laravel-be)
