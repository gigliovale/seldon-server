SELDON_KAFKA_K8S_IMAGE_VERSION=00
IMAGE_NAME=seldonio/kafka-k8s

build_image:
	docker build --force-rm=true -t $(IMAGE_NAME):$(SELDON_KAFKA_K8S_IMAGE_VERSION) .

push_to_dockerhub:
	docker login -u seldonio && \
		docker push $(IMAGE_NAME):$(SELDON_KAFKA_K8S_IMAGE_VERSION)

clean:
	@rm -fv Dockerfile


