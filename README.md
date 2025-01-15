# Student-list and Docker registry
This repo is :
 - Simple application to list student with a webserver (PHP) and API (Flask)
 - A Docker registry to manage docker image
![project](https://github.com/coulibalytech/student-list/blob/master/Docker-registry-pozos.png)
![project](https://github.com/coulibalytech/student-list/blob/master/Studentlist-Checking-pozos.png)


------------


## Objectives

The objectives of this project are to deploy Pozos application web (Frontend /Backend)  and Docker registry ( Frontend / Backend)

### Themes:

- Firstly clone the project in your repository via https://github.com/coulibalytech/student-list.git
- In your host machine mount the volume data and copy the file student_age.jsond
- Pozos web application deployment via Docker-compose or Dockerfile ( You have the choice)
- Docker private registry deployment via the commands in file (note-commande.txt)

## Context

*POZOS*  is an IT company located in France and develops software for High School.

The innovation department want to disrupt the existing infrastructure to ensure that

it can be scalable, easily deployed with a maximum of automation.

POZOS wants you to build a "**POC**" to show how docker can help you and how much this technology is efficient.

For this POC, POZOS will give you an application and want you to build a "decouple" infrastructure based on "**Docker**".

Currently, the application is running on a single server with any scalability and any high availability.

When POZOS needs to deploy a new release, every time some goes wrong.

In conclusion, POZOS needs agility on its software farm.

## Infrastructure
For this POC, you will only use one single machine with a docker installed on it.

The build and the deployment will be made on this machine.

POZOS recommends you to use centos7.6 OS because it's the most used in the company.

Please also note that you are authorized to use a virtual machine base on Centos7.6 and not your physical machine.

The security is a very critical aspect of POZOS DSI so please do not disable the firewall or other security mechanisms otherwise please explain your reasons in your delivery.

## Application

The application that you will be working on is named "*student_list*", this application is very basic and enables POZOS to show the list of the student with their age.

studen the first module is a REST API (with basic authentication needed) who send the desire list of the student based on JSON file
- The second module is a web app written in HTML + PHP who enable end-user to get a list of students

Explain  each file's role:

- docker-compose.yml: to launch the application (API and web app)
- Dockerfile: the file that will be used to build the API image (details will be given)
- requirements.txt: contains all the packages to be installed to run the application
- student_age.json: contain student name with age on JSON format
- student_age.py: contains the source code of the API in python
- index.php: PHP  page where end-user will be connected to interact with the service to - list students with age. You need to update the following line before running the website container to mak$



