# Angular SpringBoot CRUD MySQL Example

https://loizenai.com/angular-springboot-crud-mysql-example/

![Angular SpringBoot CRUD MySQL Example](https://loizenai.com/wp-content/uploads/2020/12/Angular-11-SpringBoot-CRUD-MySQL-Example.png)

Angular SpringBoot CRUD MySQL Example


 
In the tutorial, I introduce how to create an “SpringBoot Angular MySQL CRUD Example” with POST/GET/PUT/DELETE requests to SpringBoot RestAPIs.

– Design overview system by Architecture Diagram that includes: Angular Client, SpringBoot RestAPIs, and MySQL database.
– Implement Angular CRUD Client with Angular built-in HttpClient to communicate with server side.
– Implement SpringBoot RestAPIs that gets data from MySQL using Spring Data JPA and returns back data as Json format to requested Angular Client.

## Overall Angular SpringBoot MySQL CRUD Architecture Application

![Overall Angular SpringBoot MySQL CRUD Architecture Application](https://loizenai.com/wp-content/uploads/2020/06/Overall-Architecture-Angular-CRUD-Application-with-SpringBoot-Fullstack-Example.png)

- We build backend SpringBoot Application that provides RestAPIs for POST/GET/PUT/DELETE Customer entities and store them in MySQL/PostgreSQL database.
- We implement Angular Application that use Angular HTTPClient to interact (call/receive requests) with SpringBoot backend and display corresponding page view in browser.

## Overview SpringBoot CRUD MySQL Backend Architecture

![Overview SpringBoot CRUD MySQL Backend Architecture](https://loizenai.com/wp-content/uploads/2020/06/SpringBoot-RestAPIs-Backend-Architecture-Design.png)

- For building RestAPIs in SpringBoot application, we use Spring MVC Web.
- For interacting with database MySQL/PostgreSQL, we use Spring JPA.
- We implement RestAPI’s URL in RestAPIController.java file to process bussiness logic.
- For manipulating database’s records, we define a JPA model for mapping field data and use a JPA CRUD repository to do CRUD operation with MySQL/PostgreSQL.

– SpringBoot Project Structure

![SpringBoot Project Structure](https://loizenai.com/wp-content/uploads/2020/06/SpringBoot-Backend-Project-Structure.png)

- models package defines Customer model and Message response class.
- repository package defines Spring JPA repository class CustomerRepository to do CRUD operation with database.
- service package defines a middleware class CustomerServices between Controller and Repository.
- controller package defines a RestAPI Controller RestAPIController to handle POST/GET/PUT/DELETE request.

## Overview Angular CRUD Architecture Design

![Overview Angular CRUD Architecture Design](https://loizenai.com/wp-content/uploads/2020/06/Angular-CRUD-Application-Frontend-Design-Architecture.png)

Angular CRUD Application is designed with 3 main layers:

- Service Layer is used to define Angular Common Services and HttpClient Services to interact with RestAPIs
- Component Layer is used to define Angular Components to show views in Browser for interacting with Users
- Router Layer is used to route URLs mapping with the corresponding Angular Components

![Angular CRUD Application – Project Structure](https://loizenai.com/wp-content/uploads/2020/06/Angular-CRUD-Application-Project-Structure-1.png)

Angular CRUD Application defines 3 components, 2 services, 1 routers, and 2 data models:

– Components:

add-customer component is used to add a new customer to system
list-customer component is used to show all customers on view pages, delete a customer and update a customer
message component is used to define a view to show logging message on browser

– Services:

customer.service.ts defines POST/GET/PUT/DELETE HTTP requests to SpringBoot RestAPIs with the built-in Angular HttpClient.
message.service.ts defines an array storage to log all messages when Angular CRUD App running

– Router: app-routing.module.ts defines how to map a corresponding Angular component with an URL.

– Models:

customer.ts defines the main data model of our application.
message.ts defines the response data model between SpringBoot and Angular application.

## Goal – Angular SpringBoot CRUD MySQL

– Add new Customer: from Angular to SpringBoot and save to MySQL.

![– Add new Customer: from Angular to SpringBoot and save to MySQL.](https://loizenai.com/wp-content/uploads/2020/06/Angular-CRUD-App-Add-new-customers.png)

– List All Customers: from Angular calls SpringBoot RestAPI to get customer from MySQL.

![List All Customers: from Angular calls SpringBoot RestAPI to get customer from MySQL.](https://loizenai.com/wp-content/uploads/2020/06/Angular-CRUD-Application-List-All-Customer.png)


– Details a Customer: from Angular calls get http request from SpringBoot RestAPI to get a record in MySQL database

![Details a Customer](https://loizenai.com/wp-content/uploads/2020/06/Angular-CRUD-App-Details-a-Customer.png)

– Update a Customer: from Angular calls a put http request from SpringBoot RestAPI to update a record in MySQL database.

![– Update a Customer: from Angular calls a put http request from SpringBoot RestAPI to update a record in MySQL database.](https://loizenai.com/wp-content/uploads/2020/06/Angular-CRUD-Application-Update-a-Customer.png)

– Delete a Customer: from Angular calls a delete http request from SpringBoot RestAPI to delete a record in MySQL database.

![– Delete a Customer: from Angular calls a delete http request from SpringBoot RestAPI to delete a record in MySQL database.](https://loizenai.com/wp-content/uploads/2020/06/Angular-CRUD-App-Delete-a-Customer-successfully.png)

– Check database records: do a get request from Angular to SpringBoot RestAPI.

![Angular CRUD App – Check database records](https://loizenai.com/wp-content/uploads/2020/06/Angular-CRUD-App-Check-database-records.png)

## Video Guide – Angular SpringBoot CRUD MySQL Example FullStack DEBUG

https://youtu.be/848fOT3Jt44

## Related post

- [Spring Boot Security JWT Authentication Example](https://loizenai.com/spring-boot-security-jwt-authentication-example-mysql-postgresql-spring-jpa-restapis/)
- [Angular Spring Boot JWT Authentication Example](https://loizenai.com/angular-spring-boot-jwt-authentication-example-angular-6-8-9-spring-security-mysql-postgresql/)
- [Angular Django CRUD RestAPIs Application Examples](https://loizenai.com/angular-django-crud-restapis-application-examples-fullstack-angular-10-django-mysql-postgresql/)
