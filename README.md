# jenkinsDocker
Jenkins docker-compose files with dind and without it


go to jenkins-dind use CLI command: docker-compose up -d  
jenkins:lts container and dind should start.
Download some plugins:
Docker Pipeline
Docker plugin


I used this repo to test it:
https://github.com/Wyrzel/WeWillSeeHowIKnowJenkins

Add You credentials for github and dockerhub.
In nodes>configure clouds> pick docker, and fill necessery fields (for Docker Host URI put "tcp://dind:2375", its tcp adress of dind container)
For docker Agent template I used "rammydf/dind-jenkins-agent", You can use different one.
