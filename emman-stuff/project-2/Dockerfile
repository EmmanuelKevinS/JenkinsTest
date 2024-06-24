FROM centos:7

USER root

RUN yum -y update && \
    yum -y install epel-release && \
    yum -y install python36 python36-pip && \
    yum clean all

RUN python3.6 --version && pip3 --version

RUN mkdir -p /myApp

COPY hello-world.py /myApp/

WORKDIR /myApp

ENTRYPOINT ["python3.6", "hello-world.py"]
