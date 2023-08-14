Kraft Challenge
---------------

This is the main repo of the Kraft Challenge, here will be the docker compose file for 
up all the containers and is the folder that will be for all the other Kraft components.

First off you will need to clone this repo
```bash
$ git clone https://github.com/mahauni/KraftChallenge
$ cd KraftChallenge 
```

After cloning the repo and changing the directory to the KraftChallenge, you will need to clone all the
other repos.
```bash
$ git clone https://github.com/mahauni/KraftAPI
$ git clone https://github.com/mahauni/KraftApp
$ git clone https://github.com/mahauni/KraftService
```

After cloning the repos, you will need to build the .jar of the java, so you will need to use maven
for that.



After building the java projects, you will be able to docker compose the components to use the Kraft App,
so to make all the components to run you should do:
```bash
$ docker compose up -d
```

and then in your local machine, with windows, in your browser:
http://localhost/app <br>
or in linux you will have to use the ip the that your docker is using:
http://[docker_ip]/app <br>


After you are done with the application you can stop the docker container and remove all the docker image with:
```bash
$ docker-compose down && docker image rm tomcat-webapp ...
```


### Done:
- [x] Connection to the database
- [x] All main.java.esgManager.database.DAO for our tables and main.java.esgManager.entities
- [x] Crated custom data structures for our application (Linked lists for our sprint)
- [x] Created simple pool of connections to our database
### Doing:
- [ ] Trying to build up a tomcat website using docker.
- [ ] If tomcat be too hard, change to WASM or other thing.
### TODO:
- [ ] Create a display of data
- [ ] Create a script to make all the Tables and relations for postgres.
- [ ] Create test (unit, integration test) for our entire application.
- [ ] Create custom main.java.esgManager.errors and replace it in our codebase.
- [ ] Create graphs in python to show the results of our data.
