# simple-RESTful-web-service
Tutorial: Developing a RESTful API with Go and Gin


# run project go run  'fileName' or  go run .

 look at the endpoints with curl:


# post a new album with curl in a new terminal 

 curl http://localhost:8080/albums \
     --include \
     --header "Content-Type: application/json" \
     --request "POST" \
     --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'


# GET an album by ID

 curl http://localhost:8080/albums/2   where  2 => id



# GET albums

 http://localhost:8080/albums


# if it works the endpoint should be return something like :

in a terminal, run:

 $ curl http://localhost:8080/albums  

 [
    {
        "id": "1",
        "title": "Blue Train",
        "artist": "John Coltrane",
        "price": 56.99
    },  
    {
        "id": "2",
        "title": "Jeru",
        "artist": "Gerry Mulligan",
        "price": 17.99
    },  
    {
        "id": "3",
        "title": "Sarah Vaughan and Clifford Brown",
        "artist": "Sarah Vaughan",
        "price": 39.99
    },  
    {
        "id": "4",
        "title": "The Modern Sound of Betty Carter",
        "artist": "Betty Carter",
        "price": 49.99
    }
 ]

