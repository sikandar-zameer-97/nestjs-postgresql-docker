<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

## Run Project
```bash
docker compose up
```

## Stop Project
```bash
docker compose down
```

## PGADMIN4
```bash
https://localhost/login?next=/
```
credentials:
username: user-name@domain-name.com
password: strong-password

After successfull login -> Servers -> POC PostgreSQL Server -> password = password -> db

```bash
select * from book
```

## GET Endpoint
```bash
curl  -X GET \
  'http://localhost:9004/book' \
  --header 'Accept: */*' \
  --header 'User-Agent: Thunder Client (https://www.thunderclient.com)'
```

## POST Endpoint
```bash
curl  -X POST \
  'http://localhost:9004/book' \
  --header 'Accept: */*' \
  --header 'User-Agent: Thunder Client (https://www.thunderclient.com)' \
  --header 'Content-Type: application/json' \
  --data-raw '{
  "bookName": "string 4",
  "author": "string 4",
  "releaseDateTime": "2024-05-08T22:23:28.319Z",
  "createDateTime": "2024-05-08T22:23:28.319Z",
  "updateDateTime": "2024-05-08T22:23:28.319Z"
}'
```

## Miscellaneous - Not Required

```bash
npm install
```

## Generate Controller, Providers, Modules Classes
```bash
nest -- generate controller book
nest -- generate service book
nest -- generate module book
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## License

Nest is [MIT licensed](LICENSE).
