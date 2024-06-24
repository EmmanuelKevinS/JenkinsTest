IMAGE_NAME=emman-v3
IMAGE_TAG=latest
LOCAL_IMAGE_PREFIX=harbor.data.ventitechnologies.net/venti

docker-build:
	docker build -t $(LOCAL_IMAGE_PREFIX)/$(IMAGE_NAME):$(IMAGE_TAG) .

docker-push:
	docker push $(LOCAL_IMAGE_PREFIX)/$(IMAGE_NAME):$(IMAGE_TAG)

docker-push-local:
	docker tag $(IMAGE_NAME):$(IMAGE_TAG) $(LOCAL_IMAGE_PREFIX)/$(IMAGE_NAME):$(IMAGE_TAG)
	docker push $(LOCAL_IMAGE_PREFIX)/$(IMAGE_NAME):$(IMAGE_TAG)
  