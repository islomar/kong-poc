# Kong Proof of Concept
Playground for learning about Kong


## General information
* Current version (05/07/2019): 1.2.1
* Kong is a scalable, open source API Platform (also known as an API Gateway, or API Middleware, or Service Mesh for Microservices). Kong was originally built by Kong Inc. (formerly known as Mashape) to secure, manage and extend over 15,000 Microservices for its API Marketplace, which generates billions of requests per month.
* Kong is an open-source API gateway and microservice management layer.
* Based on Nginx and the lua-nginx-module (specifically OpenResty), Kong’s pluggable architecture makes it flexible and powerful.
* Kong also offers a Kubernetes Ingress Controller ready to use in your K8S environment.


## Features
- Load Balancing
- API Authentication, ACL
- Rate limiting
- Caching
- Transformations (e.g. JWT)
- Track access
- Cryptography
- Monitoring
- Logging
- Routing    
- Admin API


## Installation
* First, Kong requires a running Cassandra cluster (3.x+) or PostgreSQL instance (9.6+) before it starts. You can either use the official Cassandra/PostgreSQL containers, or use your own.
* https://hub.docker.com/_/kong 
* If you change your custom configuration, you can reload Kong (without downtime) by issuing: `docker exec -it kong kong reload`


## Kong Admin GUI
* https://github.com/pantsel/konga
* [docker-compose.yml](https://gist.github.com/pantsel/73d949774bd8e917bfd3d9745d71febf)


## Questions
* Why Kong and not Amazon API Gateway? Money? Customization?


## Resources
* https://docs.konghq.com/
* https://www.baeldung.com/kong
    - https://github.com/eugenp/tutorials/tree/master/spring-boot?
    - https://github.com/eugenp/tutorials/blob/master/spring-boot/src/main/java/com/baeldung/kong/QueryController.java
* https://medium.com/@far3ns/kong-the-microservice-api-gateway-526c4ca0cfa6