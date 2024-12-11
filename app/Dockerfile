FROM golang:1.23
RUN apt-get update && apt-get install -y iputils-ping && rm -rf /var/lib/apt/lists/*
COPY . .
RUN go build -o server .
CMD [ "./server" ]