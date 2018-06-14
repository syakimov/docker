Containers have their network and IP address
Map exposed container ports to ports on the host machine

Manually      map container ports `-p #{HOST_PORT}:#{CONTAINER_PORT}`
Automatically map container ports `-P` (expose some random host port)

`docker run -d -p 8080:80 nginx:1.7`
`docker run -d -P nginx:1.7`
