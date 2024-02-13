
![Logo](https://miro.medium.com/v2/resize:fit:700/0*R60lnmJl4hanOBaJ.png)


## Tech Stack


**Server:** Spring Boot

**Databases**: MySQL, PostGreSQL, MongoDB

**Observers** : Open Telemetory,Grafana,Prometheus,Zipkin,Loki,Grafana Tempo


## Documentation

This is project regarding hotel management which contains User , Hotel and Rating Service. Also along with that we are using Eureka netflix discovery server , Config Server , Spring API Gateway.

We have to run the Config Server first after that we have to run the Discovery or registery server.

After that we have to spin up all the services and in the end we have to spin up the API Gateway.

In the project we have used Okta Authentication. Also In the User Service we have integrated the Micrometer to get the metrics and spans. We are collecting data using the opentelemetory collector and displaying our data to grafana dashboard. To run the architecure we need to use the docker compose.

To run the Spring Application go to project root directory and use the below command: 

```mvn spring-boot:run```

To run the Infra of Micrometer Use the below command:
```docker-compose up -d ```