# create table stocks with 5 columns

SQL> create table stock
  2  (
  3  stockid int,
  4  stockname varchar(50),
  5  number_of_stocks int,
  6  country varchar(50),
  7  stock_date date
  8  );

Table created.

# create table sales with 5 columns

SQL> create table sales
  2  (
  3  saleid int,
  4  cust_name varchar(50),
  5  cust_city varchar(30),
  6  order_no int,
  7  sale_date date
  8  )
  9  ;
# create table employee
create table emp(slno int,emp_id int,join_date date,phone int,dept varchar(20));
insert into emp values(1,11,TO_DATE('10-03-1999','DD-MM-YYYY'),9942983420,'abc');
insert into emp values(2,12,TO_DATE('01-05-2001','DD-MM-YYYY'),9487983463,'def');
insert into emp values(3,13,TO_DATE('11-02-2002','DD-MM-YYYY'),9239878926,'ghi');
insert into emp values(4,14,TO_DATE('18-03-2003','DD-MM-YYYY'),9237498373,'jkl');
select * from EMP;

SLNO EMP_ID     DATE         PHONE       COMPANY
------------ ---------    ----------      --------------------
    1 11      10-MAR-99      9942983420   abc
    2 12      01-MAY-01      9487983463   def
    3 13      11-FEB-02      9239878926   ghi
    4 14      18-MAR-03      9237498373   jkl
         

SQL> desc EMP;
 Name                                      Null?    Type
 ----------------------------------------- -------- ----------------------------
SLNO                                                NUMBER(38)
EMP_ID                                              DATE
JOIN_DATE                                           NUMBER(38)
PHONE                                               NUMBER(38)
DEPT                                                VARCHAR2(20)

# display current date and time
  select to_char(sysdate,'DD/MM/YYYY hh:mi:ss') as DateTime from dual;

DATETIME
-------------------
26/04/2021 03:33:53

 display current date
SELECT sysdate from dual;

SYSDATE
---------
26-APR-21

# display current date in DD/MM/YYYY format
select to_char(sysdate,'DD/MM/YYYY') as "Date" from dual;

Date
----------
26/04/2021

# display current day as Monday
select to_char(sysdate,'Day') as Day from dual;

DAY
------------------------------------
Monday


# display date after 10 days from the current date
 SELECT sysdate+10 as "Date+10" from dual;

Date+10
---------
06-MAY-21
