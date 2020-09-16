# SpringMvc_User_Login_Registration

Create maven project:-

Steps to run project -

Right-click the application and Maven->clean.

Right-click the application and Maven->install.

Right-click the application and Run As->Run on Server->Run using Tomcat


=========================================================================

DataBase used Mysql-8.0 (Please edit Pom file according to your mysql connector/version if missmatch it will throw exception)

Datbase entries:-

CREATE DATABASE IF NOT EXISTS myusers;
USE myusers;

DROP TABLE IF EXISTS `myusers`.`users`;
CREATE TABLE `myusers`.`users` (
  `username` VARCHAR(45) NOT NULL,
  `password` VARCHAR(45) NULL,
  `firstname` VARCHAR(45) NOT NULL,
  `lastname` VARCHAR(45) NULL,
  `email` VARCHAR(45) NULL,
  `address` VARCHAR(45) NULL,
  `phone` INT NULL,
  PRIMARY KEY (`username`));
  
INSERT INTO table_name VALUES ('Ramesh',1234,'ramaesh','B','RB@gmail.com','Mumbai',902810101);
==========================================================================================================

Note:- if you get any error regarding Maven dependancy tomcat plugin then add tomcat plugin dependancy in pom.xml file and also check By 
Right click on project-properties-Deployment_Assembly-Add-Java build path entries-select MavenDependancies.
===========================================================================================================

