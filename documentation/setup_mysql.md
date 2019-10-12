# Setting up MySql on Ubuntu

```bash
sudo apt-get update
sudo apt-get -y install mysql-server

# Then enter the mysql client command prompt
sudo mysql
```

Next, create the database and MySQL user account for use in your software:

```sql
create database desolation;

CREATE USER 'desolate'@'localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON desolation.* to 'desolate'@'localhost';
```

The new user 'desolate' will now be able to log into the 'desolation' database and perform tasks such as creating tables and views as well as querying the database.

(Note - it is good practice to have different users with different permissions, e.g. this account to create the database and a different account that is only able to enter / select data)
