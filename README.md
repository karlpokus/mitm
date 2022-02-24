# mitm
Let's keep some test data in this repo

# mtls
clone these
- github.com/karlpokus/mtls
- github.com/karlpokus/prxy

````bash
# run proxy
$ go run cmd/main.go localhost:8988 localhost:8989
# run server on port 8989
$ go run server.go
# call mitm
$ curl --key cert/client/key.pem --cert cert/client/cert.pem --cacert cert/server/cert.pem https://localhost:8988/hello -v
````
