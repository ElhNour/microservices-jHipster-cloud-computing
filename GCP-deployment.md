# 2.  Deployment of Microservices with JHipster on GCP
## 2.1  Push Docker images to Docker Hub
After building docker images in the previous step, we put them on a public Docker Hub repository "nsmasteringmicroservice/tuto-store" so that the Kubernetes cluster will be able to pull them to create the containers.

![docker-hub](./imgs/1.docker-hub.png)
## 2.2  Deploy Docker containers on a Kubernetes cluster
Running the generated script "kubectl-apply.sh" with the -f option deploys the containers on the cluster. Note that some Custom Resource Definitions should be added to make Prometheus and Grafana work.

![kubectl-apply](./imgs/2.kubectl-apply.png)
## 2.3 Access the deployed app
And here is how the deployed gateway looks like!

![gateway-public](./imgs/4.gateway-deployed.png)
