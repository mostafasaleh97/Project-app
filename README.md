# Project-app
This is repo is the deployment app of my graduation project.
It contains the following:
-Files of my app using python and falsk
-Dockerfile to dockarize my app during CICD
-Jenkinsfile to run pipeline using jenkins using the repo link.
Deployment files to deploy the app in the private cluster in GCP gke.

I first write simole app using python and flask and tried it locally.
secondly, I wrote this dockerfile.
then, I write the deployment files (deployment and service using loadbalancer type to have an external ip to run in private cluster).
Finally, I write jenkinsfile than contains two stages :
the first to build dockerfile and push it on my public dockerhub.
the second to deploy files in my cluster using secret file credientials to enable jenkins to access my cluster by passing kubeconfig configuration to him in congig file.

Note: all mentioned files are found in this repo