# WireMock sample application with stub
Run WireMock sample with stubbing in docker or docker-compose.

## Start WireMock sample app with docker
Move to repository root directory
```bash
cd wiremock-sample
```
Execute docker command to run WireMock sample app.
```bash
docker run -it -p 8080:8080 wiremock/wiremock -v $(pwd)/wiremock/mappings:/home/wiremock/mappings
```

## Start WireMock sample app with docker-compose
Move to docker-compose directory.
```bash
cd docker-compose
```
Execute docker-compose command to run WireMock sample app.
```bash
docker compose up
```

## Check stub on browser
[http://localhost:8080/__admin/mappings](http://localhost:8080/__admin/mappings)

## Check stub by using curl
`curl -XGET http://localhost:8080/__admin/mappings`
