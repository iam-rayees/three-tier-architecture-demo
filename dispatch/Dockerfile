FROM golang:1.22

WORKDIR /go/src/app

COPY go.mod go.sum ./
RUN go mod download

COPY *.go ./

RUN go build -o dispatch

CMD ["./dispatch"]
