FROM debian:bookworm

RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get upgrade -y && \
	DEBIAN_FRONTEND=noninteractive apt-get install -y \
	python3 \
	ansible \
	ansible-lint \
	build-essential \
	curl \
	git \
	gnupg \
	golang-go \
	jq \
	nodejs \
	npm \
	python3-pip \
	rsync \
	ruby-rubygems \
	ruby-dev

ENV PATH=/root/.local/bin:${PATH}

RUN python3 -m pip install --user pre-commit

RUN git clone https://gitlab.com/danielfdickinson/debian-libvirt-ansible-dfd.git && \
	cd debian-libvirt-ansible-dfd && \
	chmod 0700 . && \
	pre-commit install --install-hooks && \
	cd .. && \
	rm -rf debian-libvirt-ansible-dfd
