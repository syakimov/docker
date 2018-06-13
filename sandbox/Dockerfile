# Build with `docker build -t syakimov/testimg:1.0 .`
# Run it with `docker run -it syakimov/testimg:1.0 bash`
FROM ubuntu:14.04
RUN apt update && apt install -y curl \
                                 vim

# CMD ping 127.0.0.1 -c 30
# CMD ["ping", "127.0.0.1", "-c", "30"] as json array

ENTRYPOINT ["ping"]
