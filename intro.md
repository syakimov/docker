Containters
  do not have OS
  interact with the OS kernel
  lightweight


engine(deamon)
  uses the Linux kernel to manage containters

hub
  app store for docker (contains repos for ubuntu, postgre...)

machine
  provisions docker hosts and installs the docker engine on them

swarm
  clusterss many Engines and schedules containters

compose
  manage multi-container apps

stopping the proces on the container stops the container

docker run -it ubuntu:14.04 /bin/bash
-t root user
-i interactive?

docker run -d image process (detached mode)

inspect the log of a container
  docker logs #{sha}
  docker logs -f #{sha} / same like tail -f

map the ports the container exposes to the ports on the host

there is a default cmd on every image and it is run if no cmd is passed
before trying to install something on docker with `apt` first run `apt update`
