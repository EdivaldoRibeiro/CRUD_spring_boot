# CRUD_spring_boot
Meu aprendizado fazendo CRUD usando spring_boot e postgres

##### Instalação do postgres no Ubuntu 18.04

- sudo apt update
- sudo apt install postgresql postgresql-contrib
- sudo -i -u postgres
- psql
- create database edidb1;
- create user edi with encrypted password 'edi';
- grant all privileges on database edidb1 to edi;
```
  create table employees (
  id serial,
  first_name varchar,
  last_name varchar,
  email_address varchar);
```
