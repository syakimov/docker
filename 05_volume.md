<!-- 39:01 https://training.docker.com/docker-fundamentals -->

Volume changes are ignored when committing a container
Persists when container is deleted
Can be mapped to a host folder
Can be shared between containers
Volume paths are absolute


Changes made by this container will remain after you delete container
  `docker run -itv /tmp:/test/tmp tomcat:7`
  `docker run -d -P -v /myvol tomcat:7`
