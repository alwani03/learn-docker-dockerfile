FROM golang:1.18-alpine

WORKDIR /app

RUN addgroup -S nagahitam
RUN adduser -S -D -h /app alwani nagahitam
RUN chown -R alwani:nagahitam /app

USER alwani

COPY main.go /app

EXPOSE 8080
CMD go run /app/main.go