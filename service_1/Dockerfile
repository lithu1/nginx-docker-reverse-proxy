FROM golang:1.22-alpine

WORKDIR /app
COPY . .

RUN go build -o server main.go

EXPOSE 8001
CMD ["./server"]
