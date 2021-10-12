# This Project is a sample project to study
reference: https://golang.org/doc/tutorial/web-service-gin

## How to run
```shell
go run .
```

## API list
- GET    /albums
  - You can get list of albums.
- GET    /albums/:id
  - You can get information about a single album.
- POST   /albums
  - You can add new album.

## How to use
### Get /albums
```shell
$ curl http://localhost:8080/albums 
```

### Get /albums/:id
```shell
$ curl http://localhost:8080/albums/2
```

### Post /albums
```shell
$ curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```
*In this project, there is no DB. So, result of this `post` method is only applied temporarily.*
