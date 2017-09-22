Ever wondered why we need a app/web server, configurations & other mess in order to kick start a web application? here comes Spring Boot comes to rescue.

Spring Boot makes it easy to create stand-alone, production-grade Spring based Applications that you can "just run". We take an opinionated view of the Spring platform and third-party libraries so you can get started with minimum fuss. Most Spring Boot applications need very little Spring configuration

Features or Spring Boot

Create stand-alone Spring applications
Embed Tomcat, Jetty or Undertow directly (no need to deploy WAR files)
Provide opinionated 'starter' POMs to simplify your Maven configuration
Automatically configure Spring whenever possible
Provide production-ready features such as metrics, health checks and externalized configuration
Absolutely no code generation and no requirement for XML configuration


This project is the best example for  Spring Boot + AngularJS + Spring Data + JPA CRUD


pre-requisites

make sure you configure your local datbase properties correctly in application.yml file

make sure that you execute below database scripts.


create table APP_USER (
   id BIGINT NOT NULL ,
   name VARCHAR(30) NOT NULL,
   age  INTEGER NOT NULL,
   salary REAL NOT NULL,
   PRIMARY KEY (id)
);
   
/* Populate USER Table */
INSERT INTO APP_USER(id,name,age,salary)
VALUES (1,'Sam',30,70000);
   
INSERT INTO APP_USER(id,name,age,salary)
VALUES (2,'Tom',40,50000);

CREATE SEQUENCE  "USR_SEQ"  MINVALUE 1 MAXVALUE 9999999999999999999999999999 INCREMENT BY 1 START WITH 1000 CACHE 20 NOORDER  NOCYCLE  NOPARTITION ;


How to use in your local environment.

import the project to your eclipse as a maven project.

open SpringBootCRUDApp.java file

Run as a java application by passing below VM arguments
	-Dspring.profiles.active=prod
	
	
once application is up and running hit below url in your browser
http://localhost:8080/SpringBootCRUDApp/

detailed URL
http://websystique.com/spring-boot/spring-boot-angularjs-spring-data-jpa-crud-app-example/
