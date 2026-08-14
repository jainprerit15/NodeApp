# docker-testapp

This is a small nodejs app build to containerize it using docker.
1. Created nodeApp using nodejs(this doesnt contain any database).
2. Created mongo container and mongoexpress container within same docker netwrok.
3. Put nodeApp within same network and it was able to fetch data from mongo container without having need to set up mongo setup on our local machine.
4. Used docker compose by creating .yaml file for all 3 services namely nodeApp , mongo, mongo express in order to create and run their containers using one command : docker compose -f mongodb.yaml up -d
