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

IT can be either way deployed CD using deploy stage in codefresh to kubernetes cluster continuosly. In this assigment i used AWS as i dont have an existing cluster configured. 

I used AWS ECS fargate to deploy the container images using task definitions.

