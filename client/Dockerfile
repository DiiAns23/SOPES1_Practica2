FROM golang:1.18-alpine

WORKDIR /app/src

ENV GOPATH=/app

COPY . /app/src

RUN go build -o go-client .

EXPOSE 8080

CMD [ "./go-client" ]

### docker build --tag diians2302/api-client-grpc_201903865 .
### docker push diians2302/api-client-grpc_201903865
### docker run -p 8080:8080 --name pruebaclient diians2302/go-client