# MYSQL

### MySQL Download
1. On Google, type in `MySQL server installer`
2. Click on `Download MySQL Installer`
3. Search for the appropriate MySQL installer version for the operating system.
4. Download the full installer, approximately 300 MB size.

### MySQL Installation
1. Choose `Custom` on the Setup Type menu from installer.
2. Add `MySQL Server` from `MySQL servers` menu.
3. From `Applications` add `MySQL Workbench`
4. No `Connectors` needed.
5. From `Documentation` add `MySQL Documentation` and `Samples and Examples`.

### MySQL Configuration
1. Choose `Development Computer` in order for MySQL to use minimum memory.
2. `Use Strong Password Encryption`.
3. Create the root password and confirm.
4. Set other configurations as needed.

Once MySQL is already installed, one option to start working is through the CLI.

## MySQL Commands on the CLI

#### Create a database
`create database DB_NAME`

#### Eliminate a database
`drop database DB_NAME;`

#### Show databases
`show databases;`

#### Change to the desired database
`use DB_NAME;`

#### Create a table under a selected database
`create table TABLE_NAME(ATTRIBUTE TYPE (MAX) PROPERTY, PRIMARY KEY(ATTRIBUTE));`

#### Eliminate tables on the current database
`drop table TABLE_NAME;`

Example 1:
```
create table PERSON(
  ID INT (10) not null,
  NAME VARCHAR (20),
  LASTNAME VARCHAR (20),
  ADDRESS TEXT (20),
  PHONE INT (8),
  PRIMARY KEY (ID)
  );
```

Example 2, with an auto increment starting on 100:
```
create table PERSON(
  ID INT (10) PRIMARY KEY AUTO_INCREMENT,
  PHONE INT (8),
  ) AUTO INCREMENT = 100;
```

#### Show tables on the current database
`show tables;`

#### Show how a table is structured
`describe TABLE_NAME;`
