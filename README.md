# youtube-clone-project

This repository contains source code for the Spring Boot Angular Full Stack - Youtube Clone Project

Spring Boot Angular Project, to build a complete application from the scratch using Spring Boot and Angular, building a Video Streaming Application like Youtube.

# Functional Requirements = 
We implementing the following features in this web application:

1. User can Upload new Videos.
2. User can Upload Thumbnails for the Videos.
3. User can View Videos.
4. User can Like/Dislike a Video.
5. User can Subscribe to another User, to receive updates about future videos.
6. User can Login/Logout using Single Sign On using auth0 .
7. User can comment on Videos.
8. User can view the History of Videos he/she watched.
9. User can view the List of Videos he/she Liked.

# Technologies Used =
Spring Boot, 
MongoDB, 
Angular,
AWS S3 – to store Videos and Thumbnails.

# Frontend Architecture =
We have implemented a Component Oriented Architecture in our Angular application, which means, we try to divide each meaningful element, into a different component, in that way, we can re-use the components across different places.

# Backend Architecture =
 Spring Boot REST API, we have followed a standard 3-Layer architecture also in our backend side.

We have exposed the REST API and maintain it separately in a Presentation/Controller Layer, this layer is only deal with receiving REST calls from the clients, validating whether the requests are valid or not and then delegating the request to the Service Layer.

The Service Layer perform the actual business logic of our application, it is the core of our application. This layer not deal with storing (or) persisting of the data, this is the responsibility of the Persistency Layer

The Persistence Layer is responsible to make sure that the objects are stored properly in the database, it is not deal with any kind of business logic.

By following this layered architecture approach, we can keep the code clean and maintainable.

# MongoDB Schema
Now let’s have a look at the MongoDB schema, we maintain 2 Collections inside our Database:

1. Video – We will store the meta data related to videos.
2. User – We will store the meta data related to users.
![WhatsApp Image 2023-07-04 at 5 51 10 PM](https://github.com/sandesh300/YouTube-Clone/assets/92014891/f99a8c66-8bf9-4641-a363-c48404063990)
