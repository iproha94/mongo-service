# mongo-service

To create user
`docker compose exec -it mongo mongosh -u admin`

```
db.getSiblingDB('some-db-name')

db.createUser({
  user: 'some-username',
  pwd: 'some-password',
  roles: ['readWrite'],
});
```
