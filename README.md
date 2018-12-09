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
```
insert into employees values (nextval('employees_id_seq'::regclass),'first1', 'last1','email@email1');
insert into employees values (nextval('employees_id_seq'::regclass),'first2', 'last2','email@email2');
insert into employees values (nextval('employees_id_seq'::regclass),'first3', 'last3','email@email3');
```
##### Teste

- http://localhost:8080/api/v1/employees
