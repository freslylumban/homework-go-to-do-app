FROM golang:alpine
WORKDIR /app-be

COPY . .
ENV DB_URI="mongodb://root:mongodb-password@database:27017"
ENV DB_USER="root"
ENV DB_PASS="mongodb-password"
EXPOSE 8080
RUN go build -o /go-server
CMD ["/go-server"]
