# SpringRestDemo
==================


Problem:

 

1)            Create REST APIs endpoint with any JAVA framework ex (Spring MVC, boot, Jersy etc)

2)            API endpoints {domain}/api/getproductdetails and {domain}/api/getconfigdetails

3)            Basic Authentication should be enabled for each end points and Authentication creds should be different

4)            Return a static json response with proper response code.



Ans
===

How  to  Install  it?
=====================

At  first  download  the  SpringToolsite  from  website  https://spring.io/tools

and  install  it..

STEPS  to  Run and  Create the  Spring Toolsite Project...
==========================================================

After  that  follow  this  steps....


The  Steps  given  below   is  helpful  to  create  a  Spring boot  application

a) Go  to  Spring  tool site  and  create  using SpringStarter Project

b) After  the  Project  is  created  a  package com.example.demo and  Model package.

so  Model  package  will  contain  Bean class

and  com.example.demo  will  contain  controller class  and  websecurityconfig  class...

c) After  finishing ur  work  run  the  Spring Boot App  application

so  when you  open  the  Rest url in Google

http://localhost:8083/Config/12/Laptop/Windows

it  will  add  the  rest  data

12,Laptop,Windows

and  after  that  when  you  open

http://localhost:8083/api/getconfigdetails

It  will  prompt  you  with  SpringSecuriy Username and  Password  for  the  firsttime only

After that you  give  username as  Admin  and  Password  as  "jemin1234"

it  will  display   the   configdetailsdata  in  the   google  browser...


d)

so  when you  open  the  Rest url in Google

http://localhost:8083/Product/Dell/12-05-2018/Laptop

it  will  add  the  rest  data

Dell,12-05-2018,Laptop

and  after  that  when  you  open

http://localhost:8083/api/getproductdetails


it  will  display   the   productdetialsdata  in  the   google  browser...



e)  When  you  did  not  give  Proper  password  or  Username 

it  will not  let  user  to  view  the  restful  services  datas..



===================================================================

The  Pom.xml file For Java10 version  contents  should  contain the  given below  dependencies....

Pom.xml
=======

<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>2.1.4.RELEASE</version>
		<relativePath/> <!-- lookup parent from repository -->
	</parent>
	<groupId>com.example</groupId>
	<artifactId>demo</artifactId>
	<version>0.0.1-SNAPSHOT</version>
	<name>demo</name>
	<description>Demo project for Spring Boot</description>

	<properties>
		<java.version>10</java.version>
	</properties>

	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>

<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-security</artifactId>
		</dependency>
		

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
		</dependency>
	</dependencies>

	<build>
		<plugins>
			<plugin>
				<groupId>org.springframework.boot</groupId>
				<artifactId>spring-boot-maven-plugin</artifactId>
			</plugin>
		</plugins>
	</build>

</project>

=============================================================================




