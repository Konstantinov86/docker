FROM golang:latest 
RUN mkdir /app 
COPY . /app
WORKDIR /app 
RUN go build dispatcher.go
CMD ./dispatcher
#HEALTHCHECK --interval=1m --timeout=3s CMD wget --quiet --tries=1 --spider http://localhost:80 || exit 1