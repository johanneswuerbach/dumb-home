VERSION := 1
IMAGE := johanneswuerbach/fritzbox_exporter

build:
	docker build -t $(IMAGE) .
	docker tag $(IMAGE) $(IMAGE):$(VERSION)

push: build
	docker push $(IMAGE):$(VERSION)
