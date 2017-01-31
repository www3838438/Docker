FROM ubuntu:16.04
MAINTAINER Jason Gegere <jason@htmlgraphic.com>

# Install packages then remove cache package list information
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get -yq install \
		wget \
		zip \
		unzip \
		vim \
		curl \
		mailutils \
		language-pack-en \
		iputils-ping \
		git && rm -rf /var/lib/apt/lists/*

# POSTFIX
RUN update-locale LANG=en_US.UTF-8
