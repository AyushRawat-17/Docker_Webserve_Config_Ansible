FROM centos:latest

RUN dnf install openssh-server -y

RUN dnf install openssh-clients -y

RUN ssh-keygen -A

RUN echo root:centos | chpasswd

CMD ["/usr/sbin/sshd","-D"]
