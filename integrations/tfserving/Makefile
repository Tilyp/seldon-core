IMAGE_VERSION=0.2
IMAGE_NAME = docker.io/seldonio/tfserving-proxy

SELDON_CORE_DIR=../../..

.PHONY: build
build: 
	s2i build . seldonio/seldon-core-s2i-python3:0.6-SNAPSHOT $(IMAGE_NAME):$(IMAGE_VERSION)

push_to_dockerhub:
	docker push $(IMAGE_NAME):$(IMAGE_VERSION)

