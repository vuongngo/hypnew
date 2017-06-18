# Hypothesis Website parent project

## Overview
- Website is composed by five docker containers
+ Nginx
+ Hypfrontend (universal React/Redux)
+ Hypbackend (nodejs/express)
+ Hypadmin (keystone.js)
+ Db (mongodb)

## Project setup
- Hypnew contains sub-modules of hypfrontend, hypbackend and hypadmin
- To sync three project into sub modules, run 
'''
git submodule update --recursive
'''

## Development
- Run all components with docker compose as 
'''
docker-compose up
'''
- externalize ips
+ db
127.0.0.1:27017
+ frontend:
127.0.0.1:3000
+ backend:
127.0.0.1:3002
+ admin:
127.0.01:3001

## Test & Production

