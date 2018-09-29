VERSION := 1
IMAGE := johanneswuerbach/homematic_exporter

build:
	docker build -t $(IMAGE) .
	docker tag $(IMAGE) $(IMAGE):$(VERSION)

push: build
	docker push $(IMAGE):$(VERSION)

test-i: build
	docker run --rm -it -v $(HOME)/config.ini:/root/config.ini $(IMAGE):$(VERSION) sh
