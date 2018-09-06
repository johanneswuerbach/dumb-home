VERSION := 1
REGISTRY := johanneswuerbach
IMAGE := $(REGISTRY)/git-sync-arm

build:
	rm -rf ./git-sync
	git clone https://github.com/kubernetes/git-sync.git
	GOARM=7 make -C git-sync container VERSION=$(VERSION) ARCH=arm BASEIMAGE=arm32v6/alpine:3.7 REGISTRY=$(REGISTRY)

push: build
	docker push $(IMAGE):$(VERSION)
