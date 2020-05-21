VERSION=python3.7-alpine3.9-pandas-scipy-scikitlearn-nltk-spacy
NAME=decibel/docker-python-data-science

default: build

tag:
	docker tag $(NAME) $(NAME):$(VERSION)
	#docker tag $(NAME) $(NAME):latest
	#git tag $(VERSION)

push:
	#git push --tags
	docker push $(NAME):$(VERSION)
	#docker push $(NAME):latest

build:
	docker build -t $(NAME) .

all:
	@echo "Makefile needs your attention"