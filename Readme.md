Hi There,

Thanks for the oppurtunity. 


In this Home assignment i pretty much tried a simple CI and deployment methods using 
1) Codefresh (for my CI pipeline) 
2) AWS ECS with Task definitions configured with my DOckerhub repo for deployments. 


There were some errors in the intial Dockerfile which i corrected during the configuration.  I tried with GIthub actions method for simple CI but it looked very straight forward
so i configured using a new tool codefresh.

FOR CI: 

I integratated github repo to codefresh for webhook commits to main branch initiate and prepare for builds.  Once the new images are built the same will be pushed to my docker hub repo 

codefresh pipeline configuration can be found from code_fresh_pipeline.yml

Codefresh URL : https://g.codefresh.io/

Docker hub public repo: https://hub.docker.com/r/ashokm07/testalz 
ashokm07/testalz


Deployment: 

there is a straight forward deployment with integrating azure AKS with pipeline for every successful build. But due to some restriction with azure account im ubale to configure by that method.  Anyway i commented that steps for your reference in the pipeline configuration 

It can be either way deployed CD using deploy stage in codefresh to kubernetes cluster continuosly. In this assigment i used AWS as i dont have an existing cluster configured. 

I used AWS ECS fargate to deploy the container images using task definitions.


Added execution log file 62afe2aa728822109e9c6c80.html for your reference. 

