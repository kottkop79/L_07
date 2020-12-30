FROM ubuntu:20.04 
RUN apt update && apt install git -y && apt install maven -y
WORKDIR /root
RUN mvn package -f /root/war-web-project/pom.xml
ENTRYPOINT cp /root/war-web-project/target/wwp-1.0.0.war /kopf_01/wwp-1.0.0.war
