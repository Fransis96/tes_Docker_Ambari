FROM centos:7

RUN sudo install -y wget && \
    wget -nv -O /etc/yum.repos.d/ambari.repo http://public-repo-1.hortonworks.com/ambari/centos7/2.x/updates/2.7.5.0/ambari.repo && \
    sudo install -y ambari-server && \
    sudo clean all

EXPOSE 8080

CMD ["ambari-server", "start"]
