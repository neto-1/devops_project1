# devops_project1 (The VProfile Project Setup Manual & Automated)

## About the Project
- Setting up a Multi Trier Web Application Stack
- Setup on Laptop/Desktop
- Baseline for further Projects
- Baseline for setting up any other similar projects locally

**Def** By Stack, we mean a collection of services connected together to create a user experience. For example, Nginx, Mysql, Apache tomcat connected together to create a social networking app.

## Problems
- Not confortable in making changes in real servers
- Local setup is complex, timw consuming and not repeatable

## Solutions
- Local setup that can be automated, repeatable, code IAAC
- R&D (reproduceable and deployeable) in your own machine/pc

## Tools
- Hypervisor like Oracle VM virtualbox
- Automation tools like Vagrant
- CLI, here we will use Git Bash
- IDE, here Sublime text or vscode

## Objectives of this Project
- Learn VM Automation Locally
- Use this Project as baseline for upcoming projects
- Practice real world project setup locally (for R&D)

## Architecture of Project Services
- NGINX, TOMCAT, RABBITMQ, MEMCACHED, MYSQL

## Architecture of Automated Setup
- Vagrant, Virtualbox, Gitbash, and some scripts & commands

## Prerequisites
- JDK 17 or 21
- Maven 3.9
- MySQL 8

## Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- Tomcat
- MySQL
- Memcached
- Rabbitmq
- ElasticSearch

##  Database
Here,we used Mysql DB 
sql dump file:
- /src/main/resources/db_backup.sql
- db_backup.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < db_backup.sql

## Settings
### 1. Memcached
You may encounter problem while setting the memcached service, so try to do this: `vi /etc/sysconfig/memcached` and update `OPTIONS="-l 0.0.0.0,::1"` to `OPTIONS="-l 0.0.0.0"` (ipv4)


