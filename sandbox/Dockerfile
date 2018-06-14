FROM ubuntu:14.04
RUN apt update && apt install -y nginx

# If you do not expose ports they will not be accessible form outside
# map exposed ports to host ports: `docker run -d -p 8080:80 nginx:1.7`
EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]
