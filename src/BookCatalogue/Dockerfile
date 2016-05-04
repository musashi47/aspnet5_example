FROM microsoft/aspnet

ENV http_proxy "http://192.168.56.1:3128"
ENV https_proxy "http://192.168.56.1:3128"

COPY . /app
WORKDIR /app
RUN ["dnu", "restore"]

EXPOSE 5004
ENTRYPOINT ["dnx", "-p", "project.json", "web"]
