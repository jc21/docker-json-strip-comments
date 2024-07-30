FROM centos:7

LABEL maintainer="Jamie Curnow <jc@jc21.com>"

RUN yum -y install epel-release \
	&& yum -y localinstall https://yum.jc21.com/jc21.rpm \
	&& yum -y install json-strip-comments \
	&& yum clean all \
	&& rm -rf /var/cache/yum \
	&& mkdir /workspace

WORKDIR /workspace
