# Latest version of centos
FROM centos:centos7
MAINTAINER z <devops@163.com>
RUN yum clean all && \
    yum -y install epel-release && \
    yum -y install git python-pip python-setuptools && \
    yum -y install PyYAML python-jinja2 python-httplib2 python-keyczar python-paramiko python2-pyvmomi sshpass && \
    yum clean all
RUN mkdir /etc/ansible/
RUN echo -e '[local]\nlocalhost' > /etc/ansible/hosts
RUN pip install ansible
