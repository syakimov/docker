Docker file
  list of instructions for building docker image (config file)
  more effective than docker commit

FROM -> base image
RUN -> cmd to execute
CMD -> If you do not specify cmd it runs the default cmd

It is recommended to use aggregation of `RUN` cmd `&&`
  -> docker commits container on each run which is useless

ENTRYPOINT -> always run on docker execute

ENTRYPOINT ["ping"]
