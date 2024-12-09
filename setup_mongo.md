# Setup MongoDB

## Create Admin User
- [https://www.mongodb.com/docs/v2.6/tutorial/add-admin-user/]
```bash
mongosh
use admin
```
```db.createUser({user: "superadmin", pwd: passwordPrompt(), roles: [ "root" ]})```

### Enable auth
- /etc/mongod.conf

edit:
```
security:
    authorization: "disabled"
```

restart
```sh
sudo service mongodb restart
```
  
[medium link](https://medium.com/mongoaudit/how-to-enable-authentication-on-mongodb-b9e8a924efac)

### Create Database User
- [https://www.mongodb.com/docs/manual/reference/method/db.createUser/]

```
db.createUser({user: "db-user-name", pwd: passwordPrompt(), roles: [{role: "readWrite", db: "database-name"}]})
```

### Connection URI
```
mongodb+srv://[username:password@]host[/[defaultauthdb][?options]]
```
