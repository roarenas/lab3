FROM debian
RUN apt update
RUN apt -y install curl openjdk-21-jdk iputils-ping git
WORKDIR /root
RUN curl -sO http://jenkins.local/jnlpJars/agent.jar
CMD ["java",'-jar agent.jar -url http://jenkins.local/ -secret 2c8a4586af3d6d7b631d964d81bcb30c5fe6d11ba323078279fa39464c378a79 -name debian -webSocket -workDir "/usr/workspace"']
#CMD ["/bin/sh"]