FROM registry.access.redhat.com/ubi9/go-toolset:1.18.9-14

COPY . .
COPY LICENSE /licenses/LICENSE
RUN go mod download

RUN go build -o ./main

ENV PORT 8081
EXPOSE 8081

CMD [ "./main" ]
