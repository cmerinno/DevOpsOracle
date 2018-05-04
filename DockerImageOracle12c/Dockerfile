FROM oraclelinux:7.4

RUN yum -y install oracle-rdbms-server-12cR1-preinstall.x86_64 && \
    yum clean all && \
    rm -rf /var/lib/{cache,log} /var/log/lastlog
