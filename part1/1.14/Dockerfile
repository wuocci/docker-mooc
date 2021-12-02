FROM golang:1.16-alpine
WORKDIR /usr/src/app
COPY /example-backend /usr/src/app
RUN go build

ENV REQUEST_ORIGIN=http://localhost:5000

CMD ["./server"]

#CMD LINE: docker build . -t backend && docker run -p 8080:8080 backend