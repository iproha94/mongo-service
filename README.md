# mongo-service

To create user

```
docker compose exec -it mongo mongosh -u admin

# input admin password from .env 

db.getSiblingDB('some-db-name')

use some-db-name

db.createUser({
  user: 'some-username',
  pwd: 'some-password',
  roles: ['readWrite'],
});
```
