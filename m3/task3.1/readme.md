**Part 1**
We have downloaded and installed MySQL Server an created 3 tables:
The first is named "students"
<img
src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/students.jpg" />

The second one is "tutoirs":
<img
src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/tutoirs.jpg" />

The third is "electives":
<img
src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/electives.jpg" />

Then we made selection:

**ORDER BY**
<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/select1.jpg" />

<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/select2.jpg" />

**COUNT**
<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/select3.jpg" />

Got list of all tables and made selection there:

<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/tables.jpg" />

Made a selection:

<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/select4.jpg" />

In this part we used command like:
```
create database <db_name>;
use <db_name>;
create table <table_name> (
	<column1>(type),
	<column2>(type),
	...
	primary key <column_name>
	);
insert into <table_name> (<column1>, ...) values (<value1>, ...);
select * from <table_name>;
```

**Part 2**
Making backup and restore of our database:

<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/dump.jpg" />

When we made a backup, we deleted some data from base:

<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/remove.jpg" />

After that we restored our database:

<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/after.jpg" />

Then we went to AWS, created database, connecred to it and created dump of our database.

Commands were used in this part:
```
mysqldump.exe -u <user_name> -p <db_name> > <dump_file_name.sql>;
mysql -u <user_name> -p <db_name> < <dump_file_name.sql>
```

**Part 3**
Created a database "Music" on DynamoDB, made selection:

<img
scr="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m3/task3.1/images/aws.jpg" />