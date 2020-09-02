# SBM Cloud Config Service
Spring Boot Microservice project.

  - [Description](#description)
  - [Docker images](#docker-images)
  - [Implementation details](#implementation-details)
    - [Properties](#properties)
    - [API calls](#api-calls)
      - [Verify available properties ](#verify-available-properties-)
      - [Get the properties not attached to a profile](#get-the-properties-not-attached-to-a-profile)
      - [Get the properties for the local profile, and the properties not attached to a profile](#get-the-properties-for-the-local-profile-and-the-properties-not-attached-to-a-profile)

## Description
The current project is part of the "Spring Boot Microservices with Spring Cloud" [Udemy course](https://www.udemy.com/course/spring-boot-microservices-with-spring-cloud-beginner-to-guru/). 

The project provides externalized configuration for principal services: [Beer Service](https://github.com/mariamihai/udemy-sbm-beer-service), 
[Beer Order Service](https://github.com/mariamihai/udemy-sbm-beer-order-service) and [Beer Inventory Service](https://github.com/mariamihai/udemy-sbm-beer-inventory-service).
It uses a [Git repository](https://github.com/mariamihai/udemy-sbm-brewery-config-repo) for the properties files.

An overview of all the projects involved can be found [here](https://github.com/mariamihai/udemy-sbm-overview).

## Docker images
Automatic building was not implemented for this project. The `latest` tag contains the best implementation considered 
appropriate to be used.

For automatic building of Docker images check the next projects:
- for [CircleCI](https://github.com/mariamihai/CIToDockerExampleProject)
- for [TravisCI](https://github.com/mariamihai/sma-overview) (all projects implemented under the "Spring Microservices in Action" book)

## Implementation details
### Properties
- the name of the application, used by Eureka and the other services 
```
spring.application.name=sfg-brewery-config
```
- application server port
```
server.port=8888
```

### API calls
#### Verify available properties 
 * __URI:__ _/application/profile_

 * __Method:__ _GET_

 * __URL params:__ <br/>
    * required: - <br/>
    * optional: - <br/>
    
 * __Success response:__
    * Code: 200 <br/>
    * Content: (TODO - response will be added)
       ``` 
       
       ```

 * __Error Response:__ -
    * __Code:__  <br/>
    * __Content:__ (TODO - response will be added)
    ``` 
    
    ```

#### Get the properties not attached to a profile
 * __URI:__ _/beer-service/default_

 * __Method:__ _GET_

 * __URL params:__ <br/>
    * required: - <br/>
    * optional: - <br/>
    
 * __Success response:__
    * Code: 200 <br/>
    * Content: (TODO - response will be added)
       ``` 
       
       ```

 * __Error Response:__ -
    * __Code:__  <br/>
    * __Content:__ (TODO - response will be added)
    ``` 
    
    ```
    
#### Get the properties for the local profile, and the properties not attached to a profile
 * __URI:__ _/beer-service/local_

 * __Method:__ _GET_

 * __URL params:__ <br/>
    * required: - <br/>
    * optional: - <br/>
    
 * __Success response:__
    * Code: 200 <br/>
    * Content: (TODO - response will be added)
       ``` 
       
       ```

 * __Error Response:__ -
    * __Code:__  <br/>
    * __Content:__ (TODO - response will be added)
    ``` 
    
    ```

