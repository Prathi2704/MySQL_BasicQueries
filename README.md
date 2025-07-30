# MySQL_BasicQueries
create database mkce;
-- drop database mkce;
use mkce;
show databases;
show tables;

create table student_details(Student_Name varchar(50), Roll_No int, Phone_No long, Email_ID varchar(100));

select * from student_details;

-- drop table student_details;

insert into student_details(Student_Name, Roll_No, Phone_No, Email_ID) values 
	('P',090,9876543210,'rp@gmail.com'),
    ('R', 097,9876543210,'pr@gmail.com');
    
    
create table staff_details(Staff_Name varchar(50), Staff_ID int, Phone_No long, Email_ID varchar(100), primary key(Staff_ID));

select * from staff_details;

-- drop table staff_details;
insert into staff_details(Staff_Name, Staff_ID, Phone_No, Email_ID) values 
	('PR',1,9876545678,'rp@gmail.com');
alter table staff_details
	add column DOB date;
insert into staff_details(Staff_Name, Staff_ID, Phone_No, Email_ID,DOB) values 
	('PR',2,9876545678,'rp@gmail.com','2004-07-02');
