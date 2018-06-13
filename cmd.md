Command Line
  docker run # runns images from dockerhub and personal
  docker images # lists all local images (all saved images from which you can continue)
  docker ps # lists all running docker images
  docker ps -a # lists all docker images
  docker commit #{container ID from `docker ps`} #{image name- syakimov/app:1.0}
    commits a image (state of a container) and creates a new container
    you can later start from there
  https://docs.docker.com/engine/reference/commandline/cli/
