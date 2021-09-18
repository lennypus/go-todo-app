FROM golang:buster
WORKDIR /todo-app
# copy package manifest(less-frequent changging server)
COPY . .
RUN go mod vendor
RUN go build -o app main.go
EXPOSE 8080
CMD ./app