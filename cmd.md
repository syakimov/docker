docker run # runns images from dockerhub and personal
docker images # lists all local images (all saved images from which you can continue)
docker ps # lists all running docker images
docker ps -a # lists all docker images
docker commit #{container ID from `docker ps`} #{image name- syakimov/app:1.0}
  commits a image (state of a container) and creates a new container
  you can later start from there
https://docs.docker.com/engine/reference/commandline/cli/

Remove image
  docker rmi image:tag
  docker rmi ubuntu:14.04 -f
  https://www.digitalocean.com/community/tutorials/how-to-remove-docker-images-containers-and-volumes
Remove container
  docker rm sha/name
Build image from docker file
  `docker build -t [repo-tag] [path]`
  [path] == context
    the docker client packs the path files in tar and sends them to Docker deamon
    search for config called Dockerfile in the root context
    -f search for diff file

  Example
    `docker build -t syakimov/hw:1.0 .`
      use ./ for context path
      build image in syakimov/#{IMAGE_NAME}:#{vERSION}
      tag it as 1.0

Start/Stop container
  docker start/stop sha (docker ps)

Start another process in a running container (start bash in prod)
  docker exec -it #{sha} bash

