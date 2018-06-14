Create container with name (called source container)
  `docker run -d --name #{CONTAINER_NAME} postgres` # CONTAINER_NAME = database

Create container with name and link it (called recipient container)
  `docker run -d -P --name #{RECIPIENT_NAME} --link #{SOURCE_NAME}:#{ALIAS} nginx`
    RECIPIENT_NAME = website, SOURCE_NAME = database, ALIAS = db

Example 1:
  `docker run -d --name database postgres`
  `docker run -d -P --name website --link database:db nginx`

Example 2:
  `docker run -d --name database postgres`
  `docker run -it --name website --link database:db ubuntu:14.04 bash`
  `cat /etc/hosts # notice the db ip map`
  `docker inspect database | grep IPAddress -w # verify container ip`
