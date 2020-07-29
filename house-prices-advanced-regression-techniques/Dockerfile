FROM registry.fedoraproject.org/f26/python3:latest
ENV NAME=fedora26-py VERSION=1 ARCH=x86_64
USER root
COPY requirements.txt /opt/app-root/src/requirements.txt
RUN yum install -y vim
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
CMD ["/bin/bash"]

