# Guide for running the code within a docker container

1- Install docker for you platform: https://docs.docker.com/engine/installation/#supported-platforms

2- Then, just run:
````bash
docker-compose up -d
````
It will take a long time the first time to build the container.

4- Run the following command to see the status of the running container:
````bash
docker-compose ps
````

5- Run the following command to look at the log:
````bash
docker-compose logs
````

6- The software reads the data from the datafiles folder, the parameters from the paramfiles folder, and write the output in the outfiles folder. You can change the command in the docker-compose file to run the right instance: n005w4_0_1-2-3-3 where n005w4_0_1-2-3-3 describes the instance (instance_history_weeks). You can change the parameters file and the timeout with environment variables (PARAM and TIMEOUT). The results are written in outfiles/n005w4_0_1-2-3-3/unixtimestamps (unixtimestamps is computed at every run).
