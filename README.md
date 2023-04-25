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

###### DEPOSIT:-
    INSERT INTO DEPOSIT VALUES ('101', 'SUNIL', 'AJNI', 5000.00, '1996-01-04');
    INSERT INTO DEPOSIT VALUES ('102', 'MEHUL', 'KAROBAGH', 3500.00,'1995-11-17');
    INSERT INTO DEPOSIT VALUES ('104', 'MADHURI', 'CHANDNI', 1200.00, '1995-12-17');
    INSERT INTO DEPOSIT VALUES ('105', 'PRAMOD', 'M.G.ROAD', 30000.00,'1996-03-27');
    INSERT INTO DEPOSIT VALUES ('106', 'SANDIP', 'ANDHERI',2000.00,'1996-03-31');
    INSERT INTO DEPOSIT VALUES ('107', 'SHIVANI', 'VIRAR', 1000.00,'1995-09-05');
    INSERT INTO DEPOSIT VALUES ('108', 'KRANTI', 'NEHRU PLACE', 5000.00,'1995-07-02');
    INSERT INTO DEPOSIT VALUES ('109', 'MINU', 'POWAI', 7000.00,'1995-08-10'); 

###### BRANCH:-
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
                     
###### CUSTOMERS:-
            insert into CUSTOMERS values('ANIL','CULCUTTA');
            insert into CUSTOMERS values('MEHUL','BARODA');
            insert into CUSTOMERS values('MANDAR','PATNA');
            insert into CUSTOMERS values('MADHURI','NAGPUR');
            insert into CUSTOMERS values('PRAMOD','NAGPUR');
            insert into CUSTOMERS values('SANDIP','SURAT');
            insert into CUSTOMERS values('SHIVANI','BOMBAY');
            insert into CUSTOMERS values('KRANTI','BOMBAY');
            insert into CUSTOMERS values('NAREN','BOMBAY');

###### BORROW:-
      insert into BORROW values('201','AJNI','VRCE',1000.00);
      insert into BORROW values('206','MEHUL','AJNI',5000.00);
      insert into BORROW values('311','SUNIL','DHARAMPEETH',3000.00);
      insert into BORROW values('321','MADHURI','ANDHERI',2000.00);
      insert into BORROW values('375','RAMOD','VIHAR',8000.00);
      insert into BORROW values('481','KRANTI','NEHRU PLACE',3000.00);
