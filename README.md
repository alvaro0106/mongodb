# mongodb
Documentacion MongoDB

### Install MongoDB 4.4
Install mongo db lapTop Lenovo 

Stop the mongod process by issuing the following command🦖

```
sudo service mongod stop

```

Remove any MongoDB packages that you had previously installed🦖

```
sudo apt-get purge mongodb-org*
```

Remove MongoDB databases and log files🦖
```
sudo rm -r /var/log/mongodb
sudo rm -r /var/lib/mongodb

```

### Then reinstall MongoDB 4.4.8
```
wget -qO - https://www.mongodb.org/static/pgp/server-4.4.asc | sudo apt-key add -

```
The following instruction is for Ubuntu 20.04 (Focal)🦖
```
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/4.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.4.list
```

**Update Apt
```
sudo apt-get update
```
Install MongoDB
```
sudo apt-get install mongodb-org=4.4.8 mongodb-org-server=4.4.8 mongodb-org-shell=4.4.8 mongodb-org-mongos=4.4.8 mongodb-org-too
```
Use :**
```
mongod --version 
```
I**f you encounter any error while using mongod**
```
sudo mkdir /data
cd /data
sudo mkdir db
sudo pkill -f mongod
```

**Use:**
```
mongod
```
**Stop, start, restart, status mongodb**
```
sudo service mongod stop
sudo systemctl restart mongod
sudo systemctl start mongod
sudo systemctl status mongod


```


