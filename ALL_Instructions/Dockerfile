FROM redhat/ubi9
LABEL version="1.0.0" maintainer="madhu"
ARG App_Version=1.0.0
ENV APP_PORT=8080
WORKDIR /app
COPY . /app
RUN dnf install nginx -y
EXPOSE 80
USER nginx
ENTRYPOINT [ "nginx" ]
CMD [ "-g","daemon off;" ]
