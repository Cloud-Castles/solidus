# Solidus random code

Consists of three modules

## names
entrypoint: server.py
expects a GET request, returns a random name in the body.
listens on port 8000 by default

example:
```bash
curl localhost:8000
```

returns:
```<html><body><h1>Mary Jackson</h1></body></html>```

## numbers 

entrypoint: server.py
expects a GET request, returns a random number in the body
listens on port 8000 by default

example:
```bash
curl localhost:8000
```

returns:
```<html><body><h1>107</h1></body></html>```

## scale
entrypoint: server.py
Expects a POST request with a number between 1 and 100 in the body (curl -X POST -d 54 localhost:8000)
Loads all cores on the server to the percentage specified in the POST body

example:
```bash
curl -X POST -d 54 localhost:8000
```

returns:
```<html><body><h1>Loading CPU to 54 percent</h1></body></html>```
