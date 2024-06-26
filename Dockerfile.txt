FROM node:18-slim
LABEL maintainer="andycrusoe@gmail.com" version="1.0.0"

RUN npm i nodeppt -g
VOLUME ["/ppts"]
EXPOSE 8080
CMD ["nodeppt", "start", "-d", "/ppts"]
