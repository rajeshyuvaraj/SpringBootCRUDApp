This application is the best example for  combination of Spring Boot + AngularJS + Spring Data + JPA CRUD


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
