## Searching for a script or system on Linux (suspicious things 1)!!!
One of the ways to run a script or "system" on Linux is using the init.d file. If you're searching for something suspicious that has to do with systems, then just go 
```
ls -lah /etc/init.d/
```
-lah shows basically all of the recent modifications or history of the init.d file (a directory containing scripts for init states) out in a nice long list for you to peruse. 
-lah can also just generally be used for anything useful.

## SQL Server??
Usually something called 'mySQL' on Linux if it's mentioned somewhere on your README or Forensics Questions. You can access it with 'systemctl' start and stop and 'mysql'. 
You can start a SQL daemon with
```
mysqld_safe --skip-grant-tables
```
Accessing passwords for mySQL- after doing the above, go to another terminal window, make sure you are in sudo with 'sudo -i', and execute the following commands;
```
mysql -u root
select distinct(password), user from mysql.user;
```
