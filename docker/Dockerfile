FROM golang:alpine
WORKDIR $GOPATH/src/mypackage/myapp
COPY . .
RUN go get -d -v

RUN go build -o /app/cmd/site

EXPOSE 8080

ENTRYPOINT [ "/app/cmd/site" ]

