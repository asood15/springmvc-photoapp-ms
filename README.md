# springmvc-photoapp-ms
This repo contains the following microservices:
- photoapp-discovery-service: This is Eureka discovery service
- photoapp-zuul-api-gateway: This is zuul proxy server which acts as the center point to which all microservices are communicate, it has basic authentication mechanism using jwt
- photoapp-api-config-server: This is the cloud config server project that allows all changes in property files hosted remotely to be published to all microservices
- photoapp-user-service: This is one of the microservice which connects to mysql database and talks to other microservices
- photoapp-account-management-service: This is the second microservice
- PhotoAppApiAlbums: This is the thirs microservice (cloned from third person's git repo)

It uses zuul as a proxy server, ribbon for load balancing, spring cloud bus using RabbitMq, JWT token authentication, client side load balancing using rest template and feign and basics of hysterix circuit breaker for fallback

References Udemy course: https://www.udemy.com/course/spring-boot-microservices-and-spring-cloud
