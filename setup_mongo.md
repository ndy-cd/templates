# Setup MongoDB

## Create Admin User

```bash
mongosh
use admin
```
```db.createUser({user: "superadmin", pwd: passwordPrompt(), roles: [ "root" ]})```

