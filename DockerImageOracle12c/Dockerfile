FROM oraclelinux:7.4

RUN yum -y update
RUN yum -y install libaio
RUN yum -y install unzip
RUN yum -y install net-tools
#RUN yum install rlwrap
# RUN apt-get -y install libaio1 unzip rlwrap
ADD instantclient-basic-linux.x64-12.2.0.1.0.zip /
ADD instantclient-jdbc-linux.x64-12.2.0.1.0.zip /
ADD instantclient-sdk-linux.x64-12.2.0.1.0.zip /
ADD instantclient-sqlplus-linux.x64-12.2.0.1.0.zip /
RUN unzip instantclient-basic-linux.x64-12.2.0.1.0.zip
RUN unzip instantclient-jdbc-linux.x64-12.2.0.1.0.zip
RUN unzip instantclient-sdk-linux.x64-12.2.0.1.0.zip
RUN unzip instantclient-sqlplus-linux.x64-12.2.0.1.0.zip

ENV LD_LIBRARY_PATH /instantclient_12_2

# CMD /instantclient_11_2/sqlplus <user>/<password>@//xxx.yyy.eu-west-1.rds.amazonaws.com:1521/ORCL
# CMD sleep 1; rlwrap /instantclient_11_2/sqlplus $URL