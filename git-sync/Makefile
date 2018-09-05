VERSION := 1

clone:
	rm -rf ./git-sync
	git clone https://github.com/kubernetes/git-sync.git
	make -C git-sync container VERSION=$(VERSION) ARCH=arm64 BASEIMAGE=arm64v8/alpine:3.7 REGISTRY=johanneswuerbach
	docker push johanneswuerbach/git-sync-arm64:$(VERSION)
