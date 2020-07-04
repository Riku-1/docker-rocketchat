## Docker Compose for RocketChat with Nginx
It based on the [RocketChat official image](https://raw.githubusercontent.com/RocketChat/Rocket.Chat/develop/docker-compose.yml).

It's designed to run in a AWS VPC with ELB and SSL certification is supposed to be done by ELB. 
So SSL settings don't set by itself.

### Usage
commads:
```
docker-compose up -d
```

Instantly RocketChat container will launch.

### About hubot
You have to create bot account after RocketChat server launched.
(You should change ROCKETCHAT_PASSWORD in docker-compose.yml for security.)

If you don't create bot account, hubot container eternaly repeats restart.
Or if you don't need hubot, you can delete hubot container from docker-compose.yml.