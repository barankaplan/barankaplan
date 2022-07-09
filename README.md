### **Hallo an alle 👋**


indem Sie die angehängten Repositories in diesem Profil überprüfen, können Sie sich besser über den Inhalt informieren und die Projekte schneller untersuchen. Lost geht's!



### 🗒 [review my CV](https://github.com/barankaplan/barankaplan/files/9073588/Baran.Kaplan.CV.pdf) ###




### **📂 Project 1- [Microservices](https://github.com/barankaplan/kaplans-microservice/tree/deploy-to-k8s)**

  -microservices communication using spring cloud
  
  -provide communication and load balancing between microservices using eureka discovery server
  
  -databases created with postgresql, entered queries to checked with pgadmin
  
  -a more scalable communication is provided with open feign instead of using resttemplate.
  
  -used sleuth for an auto configured distributed tracing and zipkin for checking the tracing system
  
  -external load balance(main entry point) between clients and instances using api gateway
  
  -i have created a simple message queue with rabbitmq in order not to reflect the delays due to problems between services to the user.
  
  -the project was run with jar files, then docker images cretad and uploaded by using these jar files, lastly containers were created and the project was run entirely on docker.
  
  -the project was run on kubernetes for testing using minikube on docker
  
  
  
  
### **📂 Project 2-[e-commerce Website using monolithic architecture](https://github.com/barankaplan/e-commerce-kaplan)**

  <img width="504" alt="Screenshot 2022-07-07 at 09 36 38" src="https://user-images.githubusercontent.com/59101253/177718196-1e56d7f6-309e-446d-b38d-7193a79aa89b.png">

  -In this mvc-based application designed with spring boot, thymeleaf template engine is used to interact with the frontend.
  
  -frontend designed with html css bootstrap and jquery also scaled for others devices like phones and tablets
  
  -data is kept in postgresql and spring data jpa is used in data access layer
  
  -Spring RESTful Webservices used in conjunction with jQuery on the client side
  
  -includes JUnit, Spring Test, AssertJ and Mockito for unit tests and integration tests
  
  -data can be downloaded in csv, excel and pdf formats
  

<img width="697" alt="Screenshot 2022-07-07 at 10 56 32" src="https://user-images.githubusercontent.com/59101253/177734118-52d2fb30-0540-485d-8e8c-64e84c7cc984.png">

  -Certain users have certain responsibilities and role based authorizations.for example admin controls everything but salesperson can't see users and customers
  

   <img width="592" alt="Screenshot 2022-07-07 at 11 09 32" src="https://user-images.githubusercontent.com/59101253/177737033-64ccb466-8efd-482c-ba52-e8689c80a6a9.png">

   <img width="545" alt="Screenshot 2022-07-07 at 11 08 49" src="https://user-images.githubusercontent.com/59101253/177736858-2b63ea8e-7a2e-40eb-9d87-f415394a1123.png">


<img width="726" alt="Screenshot 2022-07-07 at 11 01 48" src="https://user-images.githubusercontent.com/59101253/177735237-8e854d18-9137-4c84-8f16-947aec773b61.png">

 -custom error pages 
 
 <img width="434" alt="Screenshot 2022-07-07 at 11 15 48" src="https://user-images.githubusercontent.com/59101253/177738403-5dc86bfb-4f10-4677-90e9-70debfcd10aa.png">

<img width="699" alt="Screenshot 2022-07-07 at 11 11 28" src="https://user-images.githubusercontent.com/59101253/177737471-a90c28f1-43cc-4858-a866-d88625122877.png">

<img width="331" alt="Screenshot 2022-07-07 at 11 11 45" src="https://user-images.githubusercontent.com/59101253/177737555-baf9dd43-d6a6-4e39-bfa3-29fff104dae8.png">

  -pagination , filtering and sorting
  
  <img width="641" alt="Screenshot 2022-07-07 at 11 19 40" src="https://user-images.githubusercontent.com/59101253/177739271-ed220115-5636-4bb9-b259-e2d1cd2f6649.png">

<img width="1271" alt="Screenshot 2022-07-07 at 11 15 02" src="https://user-images.githubusercontent.com/59101253/177738203-d64729a8-4201-4b82-b638-4ae1e51d90ef.png">

  <img width="847" alt="Screenshot 2022-07-07 at 11 20 22" src="https://user-images.githubusercontent.com/59101253/177739388-d0a87fa6-cb73-4f92-bfa2-5c2a3b0ca9bb.png">
  
  
  
  
  
### **📂 Project 3- [Rest Api talks with Web Service Geonames Server](https://github.com/barankaplan/kaplans-webservice)**

This application covers alost of attemps related to spring boot Fundamentals and i listes some of them below.

**Spring Boot side**

-exception handling

-basic principles like map struct
  
-different update approaches, layered architect etc.
  
-custom exception handling layer by layer

**DB Side**

-testing /database file /h2 memory DB / PostgreSQL using test containers
  
-a basic cache mechanism between entity and web service. If the address is in the DB, data is fetched directly from DB without interacting with web service.

-JDBC principles, using queries and functions in spring boot and connection with JPA repositories.

-Hibernate and JPA principles, table relations include native, jpql, repository queries.

-if a postal code is already in database ,we don't communicate with server.

**Testing Side**

-Unit and Integration tests using different databases and docker contaniners

**Security Side**

-Basic and Bearer Token

<img width="1011" alt="Screenshot 2022-07-07 at 13 37 10" src="https://user-images.githubusercontent.com/59101253/177764526-22e0e51f-7a27-406e-99a2-cdeb037fc270.png">


### **📂 Project 4- [REST API - Blog](https://github.com/barankaplan/kaplans-RESTAPI-blog/tree/09-07-aws)**

-login and signup

-memory based authentication, token-based authentication using jwt

<img width="881" alt="Screenshot 2022-07-09 at 22 35 20" src="https://user-images.githubusercontent.com/59101253/178121780-f32a1d20-0714-4759-8f97-92f694acf9d2.png">


-request validation

<img width="354" alt="Screenshot 2022-07-09 at 22 27 48" src="https://user-images.githubusercontent.com/59101253/178121553-d5d2cee6-7df3-4790-95d3-54c6865f2a6f.png">



-pagination and sorting / page no and page size are optional



-transaction management

-exception handling



-versioning apis

<img width="888" alt="Screenshot 2022-07-09 at 22 32 24" src="https://user-images.githubusercontent.com/59101253/178121676-33389397-ac68-4bf6-bc0a-c6accac9f1b6.png">

<img width="871" alt="Screenshot 2022-07-09 at 22 32 46" src="https://user-images.githubusercontent.com/59101253/178121700-5381b3cc-204c-4195-81ff-dc07b24fb2de.png">


-api documentation using swagger api

<img width="540" alt="Screenshot 2022-07-09 at 22 30 58" src="https://user-images.githubusercontent.com/59101253/178121633-c3ebeb7f-996d-4503-903a-8f3ecec143cc.png">


-deploying on aws cloud (elastic beanstalk,rds,amazon w3)

<img width="912" alt="Screenshot 2022-07-09 at 22 28 41" src="https://user-images.githubusercontent.com/59101253/178121584-5a0b22f2-bd9d-4fe9-aa85-57cce9743821.png">

<img width="556" alt="Screenshot 2022-07-09 at 22 29 26" src="https://user-images.githubusercontent.com/59101253/178121606-876eb086-50a1-473b-b599-bc6de60a8be6.png">



### **📂 Project 5- [TCP Client Server](https://github.com/barankaplan/kaplan-socket-22)**

-My library, which contains functional interfaces consumed by stream api in various methods and using factory classes on csv files, is used by the server.(for more infos please read [docx file](https://github.com/barankaplan/kaplan-socket-22/blob/master/readme-socket.docx))

-The client goes through a 3-level password system, if it keeps the server busy for more than 20 seconds, it will be kicked out automatically.

-The server can serve 100 clients asynchronously. Check the jpeg below

![IMG_DCF2F28FC3F8-1](https://user-images.githubusercontent.com/59101253/178121092-ac749950-744f-4d98-9966-58aa33f737b6.jpeg)


### **📂 Project 6- [Device-Based Content Clustering with DBSCAN And K-Prototype Algorithms in Mobile Applications](https://github.com/barankaplan/dbscan-kprot-nlp)**

-The time devices spend on apps and content are crucial factors in creating a more interactive experience and personalized content for the user. In other words, various tables, galleries, etc., in one application throughout the day. These activities are intended to be grouped according to parameters such as the time the user browses the web, likes photos, clicks on the gallery, and watches videos.

The results are proven by using hypothesis testing and summarized in the Tableau. It is revealed that it is possible to combine the wishes and tendencies of the user corresponding to the products in the market.

<img width="409" alt="Screenshot 2022-07-09 at 22 48 42" src="https://user-images.githubusercontent.com/59101253/178122161-8895baf3-634e-4431-ab6a-00df0d088c7a.png">

<img width="830" alt="Screenshot 2022-07-09 at 22 49 25" src="https://user-images.githubusercontent.com/59101253/178122203-e87385cb-7f9d-4c17-9f83-63a6e5cf96fc.png">

<img width="493" alt="Screenshot 2022-07-09 at 22 49 48" src="https://user-images.githubusercontent.com/59101253/178122215-21ceca2d-a1c5-42e4-aaee-cbd116a0e36d.png">


-for more infos please read [docx file](https://github.com/barankaplan/dbscan-kprot-nlp/blob/main/advertising%20reccomandation%20project%20per%20device.docx)


### **📂 Project 7- [Support Vector Machines](https://github.com/barankaplan/support-vector-machine)**


### **🗂 🗂 🗂 Also you can check my works related to [files](https://github.com/barankaplan/oop-files-cases),[generics](https://github.com/barankaplan/oop-generics-cases) and [exceptions](https://github.com/barankaplan/oop-exceptions-cases)**




