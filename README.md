# 2. REST-API with Golang and PostgresSQL
A web API about users management. My next challenge in golang learning path.
Techniques used: Golang, PostgresSQL, Docker

## Function
* Get User
* Get All Users
* Create User
* Update User
* Delete User

## Package Golang tools
```
module github.com/pistolbz/go-postgres

go 1.17

require (
	github.com/gorilla/mux v1.8.0 // indirect
	github.com/joho/godotenv v1.3.0 // indirect
	github.com/lib/pq v1.10.2 // indirect
)
```
## Command to create a PostgreSQL container
```
docker run -P -p 127.0.0.1:5432:5432 -e POSTGRES_PASSWORD="1234" --name pg postgres:alpine
// -P   : Publish a container's port(s) to the host
// -p   : Publish a container's port(s) to the host
```

## New Update
* Allow updateUser to change some values, no need to change all values.



Src: https://codesource.io/build-a-crud-application-in-golang-with-postgresql/