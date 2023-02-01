## 1. Generating the microservices architecture
### 1.1.  Generate Gateway application and microservices applications
![gateway](./imgs/1.0.Gateway.png)
### 1.2.  Launch microservices, jHipster registry, and gateway
The following screenshots confirm the successful creation of the microservices and the jhispter registry.
![jHipster-registry](./imgs/1.1.Jhispter-registry.png)
We can see through the gateway that all services are up and running.
![microservices](./imgs/1.3.Before-refactoring.png)
### 1.3.  Refactor the application
After having added the entities to the microservices and launching them again, we can notice them appearing in the gateway. 
![browsing](./imgs/1.4.After-refactoring.png)
Here are the outputs of browsing some examples in the dropdown shown above.
![productorder](./imgs/1.4.1.Product-order.png)
![invoice](./imgs/1.4.2.Invoice.png)
![notification](./imgs/1.4.3.Notifications.png)
### 1.4  Build Docker images
Docker images have been successfully created.
![docker-compose](./imgs/1.4.4.Docker-compose-scale.png)
### 1.5  Monitor microservices with Prometheus & Grafana
Grafana, the visualization tool, is now accessible on port 3000. It's used to display the metrics collected by Promotheus.
![grafana](./imgs/1.5.Grafana.png)
