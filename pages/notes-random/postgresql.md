# postgresql

start your notes here
## postgresql < v16

you will need the postgresql repository
```bash copy
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
sudo apt-get update
```

## create database login etc.
After installing , yoou can use the newly created user: **postgres** 

```bash copy
sudo -i -u postgres
sudo -u postgres psql
psql

psql \q #exit psql
psql \l #show 
```


```bash copy
CREATE DATABASE fossdb;
CREATE ROLE fossi WITH LOGIN PASSWORD 'fossi' CREATEDB;
GRANT ALL PRIVILEGES ON DATABASE fossdb TO fossi;
ALTER USER fossi WITH SUPERUSER;
```

todo
pga_hba