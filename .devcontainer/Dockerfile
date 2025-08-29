# Use the devcontainers base image
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Install OpenJDK 11 and Maven
RUN apt-get update \
 && apt-get install -y --no-install-recommends openjdk-11-jdk maven git ca-certificates \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*

# Set JAVA_HOME
ENV JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
ENV PATH=$JAVA_HOME/bin:$PATH
