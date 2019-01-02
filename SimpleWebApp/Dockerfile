############################
# STEP 1 build executable binary
############################
FROM golang:alpine AS builder


COPY . $GOPATH/src/HelloWorldServer/main.go
WORKDIR $GOPATH/src/HelloWorldServer/main.go

# Build the binary.
RUN go build -o /go/bin/helloSrv

CMD [ "/go/bin/helloSrv" ]