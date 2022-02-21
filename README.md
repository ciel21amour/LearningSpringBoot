# LearningSpringBoot
SpringBoot Linkedln Learning Course Exercises

Why Spring Boot??

Supports Rapid Development - speed of setup is great.
Removes boilerplate for application setup (we used to have this application web servers earlier)
No need to have application server running on my machine all the time to support my development efforts
Used for batch processing, cron jobs, ETL type work, asynchronous message system, etc.
Cloud native support. But also traditional. Thus, very versatile.


Key components : 

Embedded Tomcat 
Auto configuration of application context
Automatic servlet mappings to allow us to leverage the servlet API.
Embedded database support and hibernate /JPA dialect
Automatic controller mapping to the dispatcher servlet that will serve some specific end points that we configure


Creating a project :
Using spring initialiser - https://start.spring.io/
Using IDE
Change port using application.properties or application.yml file in resources folder. server.port=8888



Getting Started : 

The main application class where Spring Boot operations begin contains a main method. In addition to that, it is annotated as -  @SpringBootApplication
IoC Container (a.k.a. DI Container) is a framework for implementing automatic dependency injection. (Inversion of Control)

Data Access in Spring : 

Why Spring data ?

common set of interfaces
Common naming conventions
Aspected behaviour provides data access routines without developer having to write them
Provides repository and data mapping conventions - common ORM behaviour 
Developer needs to work only with objects. Mappers are dynamic.
Removing boilerplate code
Clean mechanism for swapping out data sources (only configs need change)
Allows you to focus on business logic

Key Components :
Repository interface (interacting with data access)
Entity object. (Representing table, document) (template definition)




spring.jpa.hibernate.ddl-auto=none

By adding this in application.properties file ; 
We are informing hibernate - Dont generate any tables, we have done that for you. 

