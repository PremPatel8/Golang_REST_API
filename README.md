# Golang_REST_API

> Simple RESTful API to create, read, update and delete books. Only in-memory database created so far

## Quick Start


``` bash
# Install mux router
go get -u github.com/gorilla/mux
```

``` bash
go build
./Golang_REST_API
```

## Endpoints

### Get All Books
``` bash
GET api/books
http://localhost:8000/books
```
### Get Single Book
``` bash
GET api/books/{id}
http://localhost:8000/books/1
```

### Delete Book
``` bash
DELETE api/books/{id}
http://localhost:8000/books/1
```

### Create Book
``` bash
POST api/books
http://localhost:8000/books

# Request sample
{
    "isbn":"4545454",
    "title":"Book Three",
    "author":{"firstname":"Harry",  "lastname":"White"}
}
```

### Update Book
``` bash
PUT api/books/{id}
http://localhost:8000/books/2

# Request sample
{
    "isbn":"89878987",
    "title":"Surface Detail",
    "author":{"firstname":"Ian",  "lastname":"Banks"}
}
