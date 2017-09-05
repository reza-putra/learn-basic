## Install mongodb and start as service in Ubuntu

- https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-ubuntu-16-04

## Enable Authentication in mongodb
#### Change config mongodb enable security

  ```
  $ sudo vim /etc/mongodb.conf
  ```

  lalu cari code ini

```
#security:
```
   lalu ubah menjadi
  ```
security:
authorization: "enabled"
  ```

  ini akan mengatifkan authorization pada mongodb yang secara default terdisable

#### Create user

  ```  
  $ mongo
  $ use admin
  $ db.createUser(
    {
      user: "root",
      pwd: "root",
      roles: [{role: "userAdminAnyDatabase", db:"admin"}]
    }
   )

  ```
  restart mongodb

  ```
  sudo systemctl restart mongodb
  ```

  cek status mongodb apakah sudah active
  ```
  sudo systemctl status mongodb
  ```

  terminal akan memunculkan pesan ini jika mongodb berjalan dengan benar

  ```
  ● mongodb.service
   Loaded: loaded (/etc/systemd/system/mongodb.service; enabled; vendor preset: enabled)
   Active: active (running) since Sen 2017-08-21 01:33:16 WIB; 18min ago
 Main PID: 13505 (mongod)
    Tasks: 20
   Memory: 38.0M
      CPU: 10.325s
   CGroup: /system.slice/mongodb.service
           └─13505 /usr/bin/mongod --quiet --config /etc/mongod.conf

Agu 21 01:33:16 reza-engineer systemd[1]: Started mongodb.service.
```

  login to mongo and use user Authentication

  ```
  $ use admin
  $ db.auth("nameuser", "password")
  ```
