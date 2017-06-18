# Hypothesis Website parent project

## Overview
1. Website is composed by four docker containers
+ Hypfrontend (universal React/Redux)
+ Hypbackend (nodejs/express)
+ Hypadmin (keystone.js)
+ Db (mongodb)

## Project setup
1. Hypnew contains sub-modules of hypfrontend, hypbackend and hypadmin
2. To sync three project into sub modules, run 
'''
git submodule update --recursive
'''

## Development
1. Build docker image for each module
'''
docker build -t <module_name> .
'''

2. Run all components with docker compose as 
'''
docker-compose up
'''

3. externalize ips (for components development)
+ db
127.0.0.1:27017
+ frontend:
127.0.0.1:3000
+ backend:
127.0.0.1:3001
+ admin:
127.0.01:3002

## Components

### Hypfrontend
1. UI development
2. State management
3. Animation

### Hypbackend
1. API from Mongo
2. API connect with Instagram
3. API connect with Eventbrite
4. Mail service

### Hypadmin
1. Keystone models
2. File upload/download

### DB/NGINX/ CI
1. Setting up CI for AWS ECS || Kubernetes
2. NGINX setups with Https
3. DB setup

## Test & Production


