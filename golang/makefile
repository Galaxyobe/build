REGISTRY ?= galaxyobe

IMAGE = $(REGISTRY)/build

DOCKER_TAG ?= golang_docker-19.03


docker:
	docker build -t $(IMAGE):$(DOCKER_TAG) -f docker.dockerfile .

clean:
	docker rmi -f $(IMAGE):$(DOCKER_TAG) || true