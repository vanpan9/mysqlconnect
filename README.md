
# mysqlconnect

Connect python with Mysql

### Installation
Run below command to install package

```pip install mysqlconnect```



#### prerequisite
mysql-connector-python must be installed
To install it, run below command

```pip install mysql-connector-python```

### Connect with Mysql using python

#### import
```from connectdb import mysql_db```
#### connect
```ob=mysql_db.sql("host","user","password")```

#### Check database List
Function db_list is used to show databases list
```ob.db_list```
#### Create Database
 Function create_ db is used to create a new database
        
        Parameters
        ----------
        db_name: database name
```ob.create_db(Data_base_name)```

#### Drop Database
 Function drop_ db is used to drop a database
        
        Parameters
        ----------
        db_name: database name
```ob.drop_db(Data_base_name)```

#### Create table
Function create_ table is used to create a new table
        
        Parameters
        ----------
        table_name: table name
        columns: columns names with data type and other discription in SQL format
        example-columns="CI_n INT(2),CI_m INT(2),IAC_u VARCHAR(10),IAC_v VARCHAR(10),IAC_w VARCHAR(10),CAC_u VARCHAR(10),CAC_v VARCHAR(10),CAC_w VARCHAR(10)"

```ob.create_table(table_name,columns)```

#### Insert into Table
Function insert is used to insert value in table
        
        Parameters
        ----------
        table_name: table name
        data: values to be inserted in order
```ob.insert(table_name,data)```

#### columns
Function columns is used to print columns names
        
        Parameters
        ----------
        t_name: table name
```ob.columns(t_name)```

#### Select DataBase
Function select_db is used to select a database
        
        Parameters
        ----------
        db_name: database name
```ob.select_db(db_name)```

#### Query
Function query is used to run a SQL query 
        
        Parameters
        ----------
        query: SQL query
```ob.query(query)```





## License

© 2022 Vanshika Panwar

This repository is licensed under the MIT license. See LICENSE for details.
