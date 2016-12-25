# Creates pseudo distributed hadoop 2.6.0 on Ubuntu 14.04
#
# docker build -t sequenceiq/hadoop-ubuntu:2.6.0 .

FROM spark:0.1
USER root

ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64
ENV PATH $PATH:$JAVA_HOME/bin
ENV HADOOP_HOME=/usr/local/hadoop
ENV PATH=$PATH:/usr/local/hadoop/bin:/usr/local/hadoop/sbin
ENV SPARK_HOME /usr/local/spark
ENV YARN_CONF_DIR $HADOOP_HOME/etc/hadoop
ENV PATH $PATH:$SPARK_HOME/bin:$SPARK_HOME/sbin

CMD [ "sh", "-c", "service ssh start; bash"]

EXPOSE 50020 50090 50070 50010 50075 8031 8032 8033 8040 8042 49707 22 8088 8030 7077
