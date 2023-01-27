# 5. Load injection with Gatling for demonstrating scalability
In order to demonstrate the scalability of the gateway in the case of a large request load, we used a simulation tool called Gateling that load inject the target application to observe its behavior.

As the figure below shows, the obtained results were as expected: as soon as the CPU usage increases and exceeds the 0.1 threshold (due to the excessive number of requests), the service is automatically scaled and 3 replicas were created to increase the availability.

The link to the Gatling report can be found [here](index.html).

![gatling](./imgs/7.scalability.png)
