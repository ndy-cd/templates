# Setup MongoDB

## Create Admin User
- [https://www.mongodb.com/docs/v2.6/tutorial/add-admin-user/]
```bash
mongosh
use admin
```
```db.createUser({user: "superadmin", pwd: passwordPrompt(), roles: [ "root" ]})```

