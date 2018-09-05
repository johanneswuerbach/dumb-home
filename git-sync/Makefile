VERSION := 1

clone:
	rm -rf ./git-sync
	git clone https://github.com/kubernetes/git-sync.git
	GOARM=7 make -C git-sync container VERSION=$(VERSION) ARCH=arm BASEIMAGE=arm32v6/alpine:3.7 REGISTRY=johanneswuerbach
	docker push johanneswuerbach/git-sync-arm:$(VERSION)
