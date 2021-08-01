# Copyright IBM Corp. All Rights Reserved.
#
# SPDX-License-Identifier: Apache-2.0
#
ARG NODE_VER=12.16.1
FROM node:12.16.1-alpine@sha256:fc78f7bb1a7ef84be71f8d361f7a851c6b2432e077fa3654291a928a098da4bd
RUN apk add --no-cache \
	make \
	python \
	g++;
RUN mkdir -p /chaincode/input \
	&& mkdir -p /chaincode/output \
	&& mkdir -p /usr/local/src;
ADD build.sh start.sh /chaincode/