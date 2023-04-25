<h1 align = center>Experiment - 4</h1>

## <u>Aim:-</u>
<i><b>Implement DML commands SELECT, INSERT, UPDATE and DELETE</b></i>

### Create Commands:-

##### SYNTAX:-
`create table DEPOSIT(ACTNO VARCHAR(10),CNAME VARCHAR(20),BNAME VARCHAR(20),AMOUNT NUMERIC(8,2),ADATE DATE);`

##### OUTPUT:-

      +--------+--------------+------+-----+---------+-------+
      | Field  | Type         | Null | Key | Default | Extra |
      +--------+--------------+------+-----+---------+-------+
      | ACTNO  | varchar(10)  | YES  |     | NULL    |       |
      | CNAME  | varchar(20)  | YES  |     | NULL    |       |
      | BNAME  | varchar(20)  | YES  |     | NULL    |       |
      | AMOUNT | decimal(8,2) | YES  |     | NULL    |       |
      | ADATE  | date         | YES  |     | NULL    |       |
      +--------+--------------+------+-----+---------+-------+
      
##### SYNTAX:-
    create table BRANCH(BNAME VARCHAR(20), CITY VARCHAR(20));
    
##### OUTPUT:-

    +-------+-------------+------+-----+---------+-------+
    | Field | Type        | Null | Key | Default | Extra |
    +-------+-------------+------+-----+---------+-------+
    | BNAME | varchar(20) | YES  |     | NULL    |       |
    | CITY  | varchar(20) | YES  |     | NULL    |       |
    +-------+-------------+------+-----+---------+-------+

##### SYNTAX:-
    create table CUSTOMERS(CNAME VARCHAR(20),CITY VARCHAR(20));

##### OUTPUT:-
    +-------+-------------+------+-----+---------+-------+
    | Field | Type        | Null | Key | Default | Extra |
    +-------+-------------+------+-----+---------+-------+
    | CNAME | varchar(20) | YES  |     | NULL    |       |
    | CITY  | varchar(20) | YES  |     | NULL    |       |
    +-------+-------------+------+-----+---------+-------+
##### SYNTAX:-
`create table BORROW(LOANNO VARCHAR(20),CNAME VARCHAR(20),BNAME VARCHAR(20),AMOUNT NUMERIC(8,2));`
##### OUTPUT:-
    +--------+--------------+------+-----+---------+-------+
    | Field  | Type         | Null | Key | Default | Extra |
    +--------+--------------+------+-----+---------+-------+
    | LOANNO | varchar(20)  | YES  |     | NULL    |       |
    | CNAME  | varchar(20)  | YES  |     | NULL    |       |
    | BNAME  | varchar(20)  | YES  |     | NULL    |       |
    | AMOUNT | decimal(8,2) | YES  |     | NULL    |       |
    +--------+--------------+------+-----+---------+-------+
### Insert Commands:-

###### SYNTAX:-
    INSERT INTO DEPOSIT VALUES ('100', 'ANIL', 'VREC', 1000.00, '1996-03-01');
    INSERT INTO DEPOSIT VALUES ('101', 'SUNIL', 'AJNI', 5000.00, '1996-01-04');
    INSERT INTO DEPOSIT VALUES ('102', 'MEHUL', 'KAROBAGH', 3500.00,'1995-11-17');
    INSERT INTO DEPOSIT VALUES ('104', 'MADHURI', 'CHANDNI', 1200.00, '1995-12-17');
    INSERT INTO DEPOSIT VALUES ('105', 'PRAMOD', 'M.G.ROAD', 30000.00,'1996-03-27');
    INSERT INTO DEPOSIT VALUES ('106', 'SANDIP', 'ANDHERI',2000.00,'1996-03-31');
    INSERT INTO DEPOSIT VALUES ('107', 'SHIVANI', 'VIRAR', 1000.00,'1995-09-05');
    INSERT INTO DEPOSIT VALUES ('108', 'KRANTI', 'NEHRU PLACE', 5000.00,'1995-07-02');
    INSERT INTO DEPOSIT VALUES ('109', 'MINU', 'POWAI', 7000.00,'1995-08-10'); 

###### OUTPUT:-
      +-------+---------+-------------+---------+------------+
      | ACTNO | CNAME   | BNAME       | AMOUNT  | ADATE      |
      +-------+---------+-------------+---------+------------+
      | 100   | Anil    | VREC        | 1000.00 | 1995-03-01 |
      | 101   | Sunil   | AJNI        |  500.00 | 1996-01-04 |
      | 102   | Mehul   | KAROLBAGH   | 3500.00 | 1995-11-17 |
      | 104   | Madhuri | CHANDN      | 1200.00 | 1995-12-17 |
      | 105   | Pramod  | M.G.ROAD    | 3000.00 | 1996-03-27 |
      | 106   | Sandeep | ANDHERI     | 2000.00 | 1996-03-31 |
      | 107   | Shivani | VIRAR       | 1000.00 | 1995-09-05 |
      | 108   | Kranti  | NEHRU PLACE | 5000.00 | 1995-07-02 |
      | 109   | Minu    | POWAI       | 7000.00 | 1995-08-10 |
      +-------+---------+-------------+---------+------------+

###### SYNTAX:-
            INSERT INTO BRANCH VALUES ('VRCE', "NAGPUR");
            INSERT INTO BRANCH VALUES ('AJNI', 'NAGPUR');
            INSERT INTO BRANCH VALUES ('KAROLBAGH', 'DELHI');
            INSERT INTO BRANCH VALUES ('CHANDNI', 'DELHI');
            INSERT INTO BRANCH VALUES ('DHARAMPETH', 'NAGPUR');
            ISERT INTO BRANCH VALUES ('M.G.ROAD', 'BANGALORE');
            INSERT INTO BRANCH VALUES ('ANDHERI', 'BOMBAY');
            INSERT INTO BRANCH VALUES ('VIRAR', 'BOMBAY'); 
            INSERT INTO BRANCH VALUES ('NEHRU PLACE', 'DELHI');
            INSERT INTO BRANCH VALUES ('POWAI', 'BOMBAY'); 

###### OUTPUT:-
      +-------------+----------+
      | BNAME       | CITY     |
      +-------------+----------+
      | VRCE        | NAGPUR   |
      | AJNI        | NAGPUR   |
      | KAROLBAGH   | DELHI    |
      | CHANDINI    | DELHI    |
      | DHARAMPEETH | NAGPUR   |
      | M.G.ROAD    | BANGLORE |
      | ANDHERI     | BOMBAY   |
      | VIRAR       | BOMBAY   |
      | NEHRU PLACE | DELHI    |
      | POWAI       | BOMBAY   |
      +-------------+----------+
###### SYNTAX:-
            insert into CUSTOMERS values('ANIL','CULCUTTA');
            insert into CUSTOMERS values('MEHUL','BARODA');
            insert into CUSTOMERS values('MANDAR','PATNA');
            insert into CUSTOMERS values('MADHURI','NAGPUR');
            insert into CUSTOMERS values('PRAMOD','NAGPUR');
            insert into CUSTOMERS values('SANDIP','SURAT');
            insert into CUSTOMERS values('SHIVANI','BOMBAY');
            insert into CUSTOMERS values('KRANTI','BOMBAY');
            insert into CUSTOMERS values('NAREN','BOMBAY');

   ###### OUTPUT:-
      +---------+----------+
      | CNAME   | CITY     |
      +---------+----------+
      | ANIL    | CULCUTTA |
      | MEHUL   | BARODA   |
      | MANDAR  | PATNA    |
      | MADHURI | NAGPUR   |
      | PRAMOD  | NAGPUR   |
      | SANDIP  | SURAT    |
      | SHIVANI | BOMBAY   |
      | KRANTI  | BOMBAY   |
      | NAREN   | BOMBAY   |
      +---------+----------+
###### SYNTAX:-
      insert into BORROW values('201','AJNI','VRCE',1000.00);
      insert into BORROW values('206','MEHUL','AJNI',5000.00);
      insert into BORROW values('311','SUNIL','DHARAMPEETH',3000.00);
      insert into BORROW values('321','MADHURI','ANDHERI',2000.00);
      insert into BORROW values('375','RAMOD','VIHAR',8000.00);
      insert into BORROW values('481','KRANTI','NEHRU PLACE',3000.00);

###### OUTPUT:-
      +--------+---------+-------------+---------+
      | LOANNO | CNAME   | BNAME       | AMOUNT  |
      +--------+---------+-------------+---------+
      | 201    | AJNI    | VRCE        | 1000.00 |
      | 206    | MEHUL   | AJNI        | 5000.00 |
      | 311    | SUNIL   | DHARAMPEETH | 3000.00 |
      | 321    | MADHURI | ANDHERI     | 2000.00 |
      | 375    | RAMOD   | VIHAR       | 8000.00 |
      | 481    | KRANTI  | NEHRU PLACE | 3000.00 |
      +--------+---------+-------------+---------+
      
### Select Commands:-     

###### QUERY:-
      List all data from table DEPOSIT
###### SYNTAX:-
            select * from DEPOSIT;
###### OUTPUT:-
        +-------+---------+-------------+---------+------------+
        | ACTNO | CNAME   | BNAME       | AMOUNT  | ADATE      |
        +-------+---------+-------------+---------+------------+
        | 100   | Anil    | VREC        | 1000.00 | 1995-03-01 |
        | 101   | Sunil   | AJNI        |  500.00 | 1996-01-04 |
        | 102   | Mehul   | KAROLBAGH   | 3500.00 | 1995-11-17 |
        | 104   | Madhuri | CHANDN      | 1200.00 | 1995-12-17 |
        | 105   | Pramod  | M.G.ROAD    | 3000.00 | 1996-03-27 |
        | 106   | Sandeep | ANDHERI     | 2000.00 | 1996-03-31 |
        | 107   | Shivani | VIRAR       | 1000.00 | 1995-09-05 |
        | 108   | Kranti  | NEHRU PLACE | 5000.00 | 1995-07-02 |
        | 109   | Minu    | POWAI       | 7000.00 | 1995-08-10 |
        +-------+---------+-------------+---------+------------+
###### QUERY:-
      List all data from table BORROW
###### SYNTAX:-
      select * from BORROW;
###### OUTPUT:-
        +--------+---------+-------------+---------+
        | LOANNO | CNAME   | BNAME       | AMOUNT  |
        +--------+---------+-------------+---------+
        | 201    | AJNI    | VRCE        | 1000.00 |
        | 206    | MEHUL   | AJNI        | 5000.00 |
        | 311    | SUNIL   | DHARAMPEETH | 3000.00 |
        | 321    | MADHURI | ANDHERI     | 2000.00 |
        | 375    | RAMOD   | VIHAR       | 8000.00 |
        | 481    | KRANTI  | NEHRU PLACE | 3000.00 |
        +--------+---------+-------------+---------+

###### QUERY:-
List all data from table CUSTOMERS


###### SYNTAX:-
   select * from CUSTOMERS;
###### OUTPUT:-

###### QUERY:-
List all data from table BRANCH


###### SYNTAX:-
    select * from BRANCH;
###### OUTPUT:-

###### QUERY:-
Give account no. and amount of depositors


###### SYNTAX:-
    
###### OUTPUT:-

###### QUERY:-
Give cname and account no. of depositors


###### SYNTAX:-

###### OUTPUT:-

###### QUERY:-
Give names of customers.


###### SYNTAX:-
    select CNAME from CUSTOMERS;
###### OUTPUT:-

###### QUERY:-
Give names of branches


###### SYNTAX:-
     select BNAME from BRANCH;
###### OUTPUT:-

###### QUERY:-
Give names of borrowers


###### SYNTAX:-
   select CNAME from BORROW;
###### OUTPUT:-

###### QUERY:-
Give names of customers living in city NAGPUR


###### SYNTAX:-
    select * from CUSTOMERS where city = "NAGPUR";
###### OUTPUT:-
