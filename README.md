# SpringRestDemo
==================


Problem:

 

1)            Create REST APIs endpoint with any JAVA framework ex (Spring MVC, boot, Jersy etc)

2)            API endpoints {domain}/api/getproductdetails and {domain}/api/getconfigdetails

3)            Basic Authentication should be enabled for each end points and Authentication creds should be different

4)            Return a static json response with proper response code.



Ans
===

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

