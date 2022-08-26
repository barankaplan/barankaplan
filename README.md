### **Hallo an alle 👋**

<a name="top">
  
</a>

indem Sie die angehängten Repositories in diesem Profil überprüfen, können Sie sich besser über den Inhalt informieren und die Projekte schneller untersuchen. Lost geht's!




### 🗒 [review my CV](https://github.com/barankaplan/barankaplan/files/9094616/Baran.Kaplan.CV.pdf) ###


### 📉 [skip straight to my data science projects](#login-optional-fields)


### 🛢 [a quick introduction to postgresql, if you want to check my knowledge](https://gist.github.com/barankaplan/dc0c69f15c356c2f86f32e22bf6e019c)





### [Go to  Project 1 - AnfrageDerBetriebsstelleMittelsAbkuerzung ](#pr1)
### [Go to  Project 2 - Microservices ](#pr2)
### [Go to  Project 3 - e-commerce Website using monolithic architecture ](#pr3)
### [Go to  Project 4 - Rest Api talks with Web Service Geonames Server ](#pr4)
### [Go to  Project 5 -  REST API - Blog ](#pr5)
### [Go to  Project 6 - TCP Client Server ](#pr6)
### [Go to  Project 7 - Device-Based Content Clustering with DBSCAN And K-Prototype Algorithms in Mobile Applications ](#pr7)
### [Go to  Project 8 - Support Vector Machines ](#pr8)





<a name="pr1">

</a>

### **📂 Project 1- [AnfrageDerBetriebsstelleMittelsAbkuerzung](https://github.com/barankaplan/AnfrageDerBetriebsstelleMittelsAbkuerzung)**

![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/59101253/186783858-e200c6d5-756d-45b5-b9c6-7ef038a8e4f6.gif)

-CSV-Daten wurden untersucht und es wurde entschieden, mit "Set Data Struktur" zu arbeiten, da die Werte in der RL100-Code-Spalte eindeutig
sind und die Suche durch diese Spalte bearbeitet wird.




-Es gibt leere Werte in der Spalte mit dem Namen Typ Kurz, ich wollte Informationsverlust verhindern, indem ich in diesen Abschnitten Typ Lang
verwende.







<img width="628" alt="Screenshot 2022-08-01 at 14 19 33" src="https://user-images.githubusercontent.com/59101253/182146240-185c68e5-7d97-466d-acb7-c3a0195828d0.png">

 



-Ich habe eine oberflächliche Unit-Test-Methode über die OperationOfficeFactory-Klasse geschrieben, aus der wir die CSV Daten einlesen.
Obwohl es nicht direkt mit dem Konzept des Testens zusammenhängt, wurde die Methodenvielfalt durch die Gestaltung von Validierungsbestimmungen mit Unit-Test-Methoden erhöht, und gleichzeitig wurden "Stream-Operationen" erwähnt.






<img width="744" alt="Screenshot 2022-08-01 at 14 19 00" src="https://user-images.githubusercontent.com/59101253/182146166-32f7bc57-25b8-4157-8adb-b68d3c8d0f3c.png">


 



 



-Integrationstest wurde mit einer Datenbank auf AWS durchgeführt (Details folgen später).

<img width="745" alt="Screenshot 2022-08-01 at 14 19 14" src="https://user-images.githubusercontent.com/59101253/182146195-11340839-9b30-4d22-979a-bfd81a6dc008.png">








 



-Dank der Validierungen, die während "Get Request" laufen, konnte ich die Verschwendung von Ressourcen minimieren.




 <img width="737" alt="Screenshot 2022-08-01 at 14 18 48" src="https://user-images.githubusercontent.com/59101253/182146117-0d262d2c-b055-4944-b0ac-52ac497f1790.png">




-Collection link in Postman:  https://www.getpostman.com/collections/a259b863777eadeb1f6b




<img width="745" alt="Screenshot 2022-08-01 at 14 18 34" src="https://user-images.githubusercontent.com/59101253/182146075-3cab0328-f7d9-4c0a-824c-f1b32d54257e.png">




-Im ersten und einfachen Szenario werden csv-Dateien unabhängig von einer Datenbank mit dem Pojo-Objekt namens „OperationOffice“ verarbeitet. Diese Anfrage zielt darauf ab, die gewünschte Basisleistung im Projekt darzustellen, ohne dass eine
Sicherheit verlangt wird.



 


<img width="522" alt="Screenshot 2022-08-01 at 14 18 20" src="https://user-images.githubusercontent.com/59101253/182146044-e8d597d0-8edb-4538-b00f-71a695001e7d.png">



 



-Statt Fehlerdetails wie "timestamp-status-error-trace" usw.Durch "Exception Handling"-Mechanismen werden dem Benutzer
verschiedene Fehlermeldungen angezeigt.



 

<img width="491" alt="Screenshot 2022-08-01 at 14 18 09" src="https://user-images.githubusercontent.com/59101253/182146010-a10c210d-2283-459f-8807-6c7a2d0fdc1f.png">

 



-Im zweiten Szenario wird dieselbe OperationOffice-Klasse als Entität mit einem anderen Ansatz dargestellt, indem die Datenbank-, Authentifizierungs- und Autorisierungsprozesse in einer mehrschichtigen Architektur durchlaufen werden.



 



-Eine einfache Benutzerregistrierung und ein Login-Code wurden entwickelt. Das Passwort ist verschlüsselt und die APIs Connection wird mit JWT bereitgestellt.



<img width="800" alt="Screenshot 2022-08-01 at 14 17 27" src="https://user-images.githubusercontent.com/59101253/182145912-fd081b74-ed12-45d9-a84e-356c9c303df8.png">




-Der Benutzer kann ohne das Token nicht mit dem Server kommunizieren. Als Ergebnis erfolgreicher Anmeldungen mit dem Token zurückgegebene Objekte werden
in einer Datenbank gespeichert, die sich in der AWS-Cloud befindet! Ich erwähnte, dass ich einen einfachen Integrationstest über diese Datenbank geschrieben habe!



<img width="631" alt="Screenshot 2022-08-01 at 14 16 33" src="https://user-images.githubusercontent.com/59101253/182145776-f6d79fe1-e406-4e6b-b185-daadd76f84b8.png">





-Da es sich um den Primärschlüssel Code handelt, wird Daten Wiederholung vermieden! Also selbst wenn der Benutzer dieselbe Anfrage 100-mal zu
unterschiedlichen Zeiten schreibt, wird nur 1 aufgenommen!


![image](https://user-images.githubusercontent.com/59101253/182145259-42fc0b7f-9544-4c0d-99c5-7c3721018700.png)


-In der Datei application.properties werden Logging-Level-Anpassungen für verschiedene Klassen über die Slf4j-API vorgenommen.


<img width="889" alt="Screenshot 2022-08-02 at 02 14 26" src="https://user-images.githubusercontent.com/59101253/182265613-36aee93d-ece8-4bcb-9858-31de6b8b5c2b.png">

-"Logging data" werden in einem benutzerdefinierten Format in operationOffice.log gespeichert. Die maximale Dateigröße, die maximale Gesamtgröße der Logging-Daten und die Aufbewahrungszeit werden angegeben. Der Logging-Verlauf wird bei jedem Programmstart gelöscht (er wird nicht gelöscht, wenn er innerhalb des nächsten Tages gestartet wird).

<img width="902" alt="Screenshot 2022-08-02 at 02 13 51" src="https://user-images.githubusercontent.com/59101253/182265562-d4794711-5954-4fe7-a7df-f8b8177d8fec.png">




-Es wird eine einfache Logging auf Methodenebene durchgeführt. Außerdem wird die Logging auf Methodenebene mithilfe des AOP-Ansatzes mit benutzerdefinierter Annotation entworfen!

<img width="953" alt="Screenshot 2022-08-02 at 02 12 55" src="https://user-images.githubusercontent.com/59101253/182265482-2361cb57-7ea5-431a-b877-401dfd307be3.png">


-04.08.22

-Am Anfang des Projekts stand die Idee, dass die csv-Daten sich bei jeder Abfrage möglicherweise ändern könnten, sodass wolte ich die csv-Datei direkt Zeile für Zeile einlesen, um die aktuellsten Daten zu übertragen.

<img width="717" alt="Screenshot 2022-08-05 at 00 07 06" src="https://user-images.githubusercontent.com/59101253/182960983-88bc722c-4be1-4932-beaf-9e660747cd99.png">



-Deswegen wurde nach dem einmaligen Auslesen der csv-Datei der Link http://localhost:8082/api/betriebsstelle/collection/{code} angelegt, um die Daten statisch zu halten und so die Daten in der Collection auszulesen.

<img width="675" alt="Screenshot 2022-08-05 at 00 07 29" src="https://user-images.githubusercontent.com/59101253/182961033-3bded8c1-4bdf-4073-bc59-71e1426fb3b6.png">


-Auf diese Weise wird ersichtlich, dass die Lesegeschwindigkeit durch Beobachten von Logging Daten zunimmt. Allerdings bleibt, wie anfangs erwähnt, der Status der erstmalig gelesenen Daten erhalten!

<img width="1094" alt="Screenshot 2022-08-05 at 00 07 59" src="https://user-images.githubusercontent.com/59101253/182961082-abbf3b53-d680-485a-b31d-1883cb94f18f.png">




Zusätzliche Verbesserungen



- Versioning and documentation of APIs 



- Dockerizing Jar files and run on AWS ECS



- Different Grant Types Using Oauth2

    
- Logging Operations and AOP Approach (added on 02.08.22)


- Creating custom annotations (added on 02.08.22)

     
- Spring MVC + Angular

### [Go to the top of the page ](#top)


<a name="pr2">

</a>

### **📂 Project 2- [Microservices](https://github.com/barankaplan/kaplans-microservice/tree/deploy-to-k8s)**

  -microservices communication using spring cloud
  
  -provide communication and load balancing between microservices using eureka discovery server
  
  -databases created with postgresql, entered queries to checked with pgadmin
  
  -a more scalable communication is provided with open feign instead of using resttemplate.
  
  -used sleuth for an auto configured distributed tracing and zipkin for checking the tracing system
  
  <img width="1355" alt="Screenshot 2022-07-11 at 10 37 34" src="https://user-images.githubusercontent.com/59101253/178223422-18a0533a-2fe3-46c1-8bc2-d50c143f665b.png">
  
<img width="1064" alt="Screenshot 2022-07-11 at 10 39 28" src="https://user-images.githubusercontent.com/59101253/178223769-cdaeac55-59ca-435b-8c25-f5912ac31fd2.png">

  -external load balance(main entry point) between clients and instances using api gateway
  
  -i have created a simple message queue with rabbitmq in order not to reflect the delays due to problems between services to the user.
  
  -the project was run with jar files, then docker images cretad and uploaded by using these jar files, lastly containers were created and the project was run entirely on docker.
  
  <img width="776" alt="Screenshot 2022-07-11 at 10 42 28" src="https://user-images.githubusercontent.com/59101253/178224306-3b74674c-3c88-432b-a913-6d0438273200.png">

<img width="1311" alt="Screenshot 2022-07-11 at 10 42 54" src="https://user-images.githubusercontent.com/59101253/178224395-48a1435d-80d6-48fc-8849-ca41d8014f57.png">

  
  <img width="1076" alt="Screenshot 2022-07-11 at 10 36 49" src="https://user-images.githubusercontent.com/59101253/178223274-689e1529-c381-4ba7-b06e-10a5423c1ad0.png">

  
  
  -the project was run on kubernetes for testing using minikube on docker
  
  <img width="1004" alt="Screenshot 2022-07-11 at 10 31 09" src="https://user-images.githubusercontent.com/59101253/178222256-ac419a59-95b0-4143-aad8-b0cfdfd84d1b.png">


<img width="726" alt="Screenshot 2022-07-11 at 10 30 16" src="https://user-images.githubusercontent.com/59101253/178222110-cce6d38d-7c71-402a-a20a-a683db4a8fc7.png">

  <img width="1067" alt="Screenshot 2022-07-11 at 10 34 02" src="https://user-images.githubusercontent.com/59101253/178222779-74afc976-4129-461c-a15f-5229346fc887.png">
  
<img width="1168" alt="Screenshot 2022-07-11 at 10 35 42" src="https://user-images.githubusercontent.com/59101253/178223052-91a33723-c448-4f69-82ff-fde1d8a64b1d.png">

### [Go to the top of the page ](#top)

<a name="pr3">

</a>
  
### **📂 Project 3-[e-commerce Website using monolithic architecture](https://github.com/barankaplan/e-commerce-kaplan)**

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
  
### [Go to the top of the page ](#top)
  
<a name="pr4">

</a>

  
### **📂 Project 4- [Rest Api talks with Web Service Geonames Server](https://github.com/barankaplan/kaplans-webservice-22)**

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


-let's sign in

<img width="958" alt="Screenshot 2022-07-10 at 20 04 59" src="https://user-images.githubusercontent.com/59101253/178156736-ee9f9e81-5f23-4aa4-96fa-d45fe9311fce.png">


-it is possible to create a movie info !

<img width="639" alt="Screenshot 2022-07-10 at 20 05 23" src="https://user-images.githubusercontent.com/59101253/178156738-3eb612cb-a700-4d3b-821d-a56a1b00e82b.png">


-and create an order using our card

<img width="473" alt="Screenshot 2022-07-10 at 20 06 02" src="https://user-images.githubusercontent.com/59101253/178156758-f5de6e7e-a612-448f-a285-0cee3d91a13f.png">

<img width="571" alt="Screenshot 2022-07-10 at 20 06 17" src="https://user-images.githubusercontent.com/59101253/178156766-42bc9d44-67a9-4a66-842c-229b5fe7952b.png">


-If a card has been entered into the system, it cannot be entered by another person!

<img width="499" alt="Screenshot 2022-07-10 at 20 07 39" src="https://user-images.githubusercontent.com/59101253/178156812-6073462e-81d9-49a9-86d4-cdfbb842929c.png">

-if a postal code is already in database ,we don't communicate with server.

<img width="629" alt="Screenshot 2022-07-10 at 20 09 10" src="https://user-images.githubusercontent.com/59101253/178156863-70b8ff01-22aa-4dc2-9587-eae8ed545cf7.png">

<img width="556" alt="Screenshot 2022-07-10 at 20 10 02" src="https://user-images.githubusercontent.com/59101253/178156897-5815150a-6d4c-4cb6-ab30-04701a6e8c8e.png">


### [Go to the top of the page ](#top)


<a name="pr5">

</a>


### **📂 Project 5- [REST API - Blog](https://github.com/barankaplan/kaplans-RESTAPI-blog/tree/09-07-aws)**

### [Click here to reach the version running on elastic beanstalk !](http://kaplansrestapiblog-env-2.eba-nnqctyzc.us-east-1.elasticbeanstalk.com/swagger-ui/#/)

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


<img width="727" alt="Screenshot 2022-07-10 at 10 09 23" src="https://user-images.githubusercontent.com/59101253/178136709-4e6138d1-c3cd-4e53-996c-13a1add1eb21.png">

<img width="733" alt="Screenshot 2022-07-10 at 10 10 33" src="https://user-images.githubusercontent.com/59101253/178136739-befca0a7-c8c9-4dd3-be52-34a1937c461a.png">

<img width="1407" alt="Screenshot 2022-07-10 at 10 10 52" src="https://user-images.githubusercontent.com/59101253/178136760-f10b4061-8485-460c-94f8-5f2b692f3d9a.png">

### [Go to the top of the page ](#top)


<a name="pr6">

</a>

### **📂 Project 6- [TCP Client Server](https://github.com/barankaplan/kaplan-socket-22)**

-My library, which contains functional interfaces consumed by stream api in various methods and using factory classes on csv files, is used by the server.(for more infos please read [docx file](https://github.com/barankaplan/kaplan-socket-22/blob/master/readme-socket.docx))

-The client goes through a 3-level password system, if it keeps the server busy for more than 20 seconds, it will be kicked out automatically.

-The server can serve 100 clients asynchronously. Check the jpeg below

![IMG_DCF2F28FC3F8-1](https://user-images.githubusercontent.com/59101253/178121092-ac749950-744f-4d98-9966-58aa33f737b6.jpeg)


### **🗂 🗂 🗂 Also you can check my works related to [files](https://github.com/barankaplan/oop-files-cases),[generics](https://github.com/barankaplan/oop-generics-cases) and [exceptions](https://github.com/barankaplan/oop-exceptions-cases)**


<h4 id="login-optional-fields">
Data Science Projects
</h4>


### [Go to the top of the page ](#top)


<a name="pr7">

</a>

### **📂 Project 7- [Device-Based Content Clustering with DBSCAN And K-Prototype Algorithms in Mobile Applications](https://github.com/barankaplan/dbscan-kprot-nlp)**

-The time devices spend on apps and content are crucial factors in creating a more interactive experience and personalized content for the user. In other words, various tables, galleries, etc., in one application throughout the day. These activities are intended to be grouped according to parameters such as the time the user browses the web, likes photos, clicks on the gallery, and watches videos.

The results are proven by using hypothesis testing and summarized in the Tableau. It is revealed that it is possible to combine the wishes and tendencies of the user corresponding to the products in the market.

<img width="409" alt="Screenshot 2022-07-09 at 22 48 42" src="https://user-images.githubusercontent.com/59101253/178122161-8895baf3-634e-4431-ab6a-00df0d088c7a.png">

<img width="830" alt="Screenshot 2022-07-09 at 22 49 25" src="https://user-images.githubusercontent.com/59101253/178122203-e87385cb-7f9d-4c17-9f83-63a6e5cf96fc.png">

<img width="493" alt="Screenshot 2022-07-09 at 22 49 48" src="https://user-images.githubusercontent.com/59101253/178122215-21ceca2d-a1c5-42e4-aaee-cbd116a0e36d.png">


-for more infos please read [docx file](https://github.com/barankaplan/dbscan-kprot-nlp/blob/main/advertising%20reccomandation%20project%20per%20device.docx)

### [Go to the top of the page ](#top)


<a name="pr8">

</a>

### **📂 Project 8- [Support Vector Machines](https://github.com/barankaplan/support-vector-machine)**


### **📄 [Read one of my published article covers PCA on datatab,which is one of the most popular online statistics calculator.](https://datatab.net/tutorial/pca)**





