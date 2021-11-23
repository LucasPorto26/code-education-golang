FROM golang:1.6-alpine

WORKDIR /app

COPY go.mod ./
COPY go.sum ./

#RUN go mod download

COPY *.go ./

RUN go build -o /full-cycle.go

EXPOSE 8080

CMD ["/full-cycle.go"]
