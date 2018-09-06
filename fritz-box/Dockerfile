FROM arm32v6/golang:1.10-alpine3.7

RUN apk add --no-cache git

RUN go get github.com/ndecker/fritzbox_exporter/ && \
	cd $GOPATH/src/github.com/ndecker/fritzbox_exporter && \
	go install

ENTRYPOINT ["fritzbox_exporter"]
