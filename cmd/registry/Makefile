all: build

build:
	GOOS=linux GOARCH=amd64 CGO_ENABLED=0 go build;\
	docker build --pull -t registry.bizsaas.net/registry:2.7.1.1 .

push:
	docker push registry.bizsaas.net/registry:2.7.1.1

.PHONY: all build push